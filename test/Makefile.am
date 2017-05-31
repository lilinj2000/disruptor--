
BOOST_HOME_PATH = ${HOME}/3rd/boost
BOOST_INCLUDE_PATH = ${BOOST_HOME_PATH}/include
BOOST_LIB_PATH = ${BOOST_HOME_PATH}/lib

AM_CXXFLAGS = @AM_CXXFLAGS@ -I$(top_srcdir) -I${BOOST_INCLUDE_PATH}

AM_LDFLAGS = -L${BOOST_LIB_PATH} \
			-lboost_unit_test_framework \
			-lboost_timer \
			-lboost_system \
			-lboost_chrono \
			@AM_LDFLAGS@

check_PROGRAMS = sequencer_test ring_buffer_test

sequencer_test_SOURCES = sequencer_test.cc
ring_buffer_test_SOURCES = ring_buffer_test.cc

TESTS = ${check_PROGRAMS}
