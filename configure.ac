AC_PREREQ(2.69)
AC_INIT(STM32F4_HAL, 1.0)

AC_NO_EXECUTABLES

AC_CONFIG_AUX_DIR(config)
AC_CONFIG_MACRO_DIR([m4])
AM_INIT_AUTOMAKE([foreign subdir-objects])
LT_INIT

# Use "make V=1" in order to see the gcc command-lines during compilation.
m4_ifdef([AM_SILENT_RULES],[AM_SILENT_RULES([yes])])

ARCH_FLAGS=" -mcpu=cortex-m4 -mthumb -mfloat-abi=soft"

AC_PROG_CC
AM_PROG_CC_C_O

AC_CHECK_PROGS([DOXYGEN], [doxygen])
if test -z "$DOXYGEN";
   then AC_MSG_WARN([Doxygen not found - continuing without Doxygen support])
fi

AC_MSG_CHECKING(debug build)
AC_ARG_ENABLE([debug],
              [AS_HELP_STRING([--enable-debug=[[yes/no]]],
                              [generate a non-optimized debug build [default=no]])],
              [case "${enableval}" in
               yes) debug_build=true ;;
               no)  debug_build=false ;;
               *) AC_MSG_ERROR([bad value ${enableval} for --enable-debug]) ;;
               esac],
              debug_build=false)

if [ test x$debug_build = xtrue ]
then
    AC_MSG_RESULT(yes)
    DEBUG_FLAGS="-O0 -DDEBUG -g3"
else
    AC_MSG_RESULT(no)
    DEBUG_FLAGS="-O3 -DNDEBUG"
fi

AC_MSG_CHECKING([TARGET])
AC_ARG_VAR(TARGET,
	[ STM32F4 varient to use for HAL build [default=STM32F439xx]]
)

if test "$TARGET" != "" ; then
	AC_MSG_RESULT([$TARGET]) 
	hal_target="$TARGET" 
else
	AC_MSG_RESULT([STM32F439xx])
	hal_target="STM32F439xx"
fi 
AC_SUBST(HAL_TARGET, "$hal_target")

AC_MSG_CHECKING([HSE_VALUE])
AC_ARG_VAR(HSE_VALUE,
        [ Target systems external clock speed (HSE) [default=8000000Hz]]
)

if test "$HSE_VALUE" != "" ; then
        AC_MSG_RESULT([$HSE_VALUE])    
	AC_SUBST(HSE_VALUE_OVERRIDE, "-DHSE_VALUE=$HSE_VALUE")
else
        AC_MSG_RESULT([8,000,000])
fi

CFLAGS+=" $ARCH_FLAGS $DEBUG_FLAGS -D$HAL_TARGET $HSE_VALUE_OVERRIDE"

AC_CONFIG_FILES(Makefile)
AM_CONDITIONAL([HAVE_DOXYGEN], 
[test -n "$DOXYGEN"])AM_COND_IF([HAVE_DOXYGEN], [AC_CONFIG_FILES([docs/doxyfile docs/Makefile])])

AC_OUTPUT
