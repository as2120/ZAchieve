# Makefile for ptester
# This program is free software; you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation; either version 2 of the License, or
# (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
# You should have received a copy of the GNU General Public License
# along with this program; if not, write to the Free Software
# Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.

LIBS = -lthread -lnsl -lsocket -ldl

fail:
	@echo 'NoNo! Don't run "make" in this directory!'
	@exit 1

LIBOBJS = #../phttpd/fdstdio.o ../phttpd/safeio.o
all:	ptester

ptester: ptester.o $(XOBJS)
	$(CC) -o ptester ptester.o $(XOBJS) $(LIBOBJS) $(LIBS)

clean:
	-rm -f *.o ptester
