
#  This file is part of the DSP-Crowd project
#  https://www.dsp-crowd.com

#  Author(s):
#      - Johannes Natter, office@dsp-crowd.com

#  Copyright (C) 2017 Authors and www.dsp-crowd.com

#  This program is free software: you can redistribute it and/or modify
#  it under the terms of the GNU General Public License as published by
#  the Free Software Foundation, either version 3 of the License, or
#  (at your option) any later version.

#  This program is distributed in the hope that it will be useful,
#  but WITHOUT ANY WARRANTY; without even the implied warranty of
#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
#  GNU General Public License for more details.

#  You should have received a copy of the GNU General Public License
#  along with this program. If not, see <http://www.gnu.org/licenses/>.

bin_PROGRAMS = dspc-hello

dspc_hello_SOURCES = main.cpp DspcHello.cpp

AM_CPPFLAGS = \
		-I${srcdir}/../hal \
		-I${srcdir}/include \
		-DHAVE_SSTREAM

dspc_hello_LDADD = \
		../hal/libhal.la
dspc_hello_LDFLAGS = -static

# Use dummy cpp file to ensure that hal lib is linked with g++
nodist_EXTRA_dspc_hello_SOURCES = dummy.cpp
