#
# Copyright (c) 2009 Red Hat, Inc.
# 
# Authors: Andrew Beekhof
#	   Steven Dake (sdake@redhat.com)
#
# This software licensed under BSD license, the text of which follows:
# 
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions are met:
# 
# - Redistributions of source code must retain the above copyright notice,
#   this list of conditions and the following disclaimer.
# - Redistributions in binary form must reproduce the above copyright notice,
#   this list of conditions and the following disclaimer in the documentation
#   and/or other materials provided with the distribution.
# - Neither the name of the MontaVista Software, Inc. nor the names of its
#   contributors may be used to endorse or promote products derived from this
#   software without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
# AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
# IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
# ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE
# LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
# CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
# SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
# INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF
# THE POSSIBILITY OF SUCH DAMAGE.

MAINTAINERCLEANFILES    = Makefile.in
INCLUDES       		= -I$(top_builddir)/include  -I$(top_srcdir)/include

noinst_PROGRAMS		= testevs evsbench evsverify testcpg testcpg2 cpgbench testconfdb	\
			logsysbench logsysrec testquorum testvotequorum1 testvotequorum2

testevs_LDADD		= -levs
testevs_LDFLAGS		= -L../lib
testcpg_LDADD		= -lcpg
testcpg_LDFLAGS		= -L../lib
testcpg2_LDADD		= -lcpg
testcpg2_LDFLAGS	= -L../lib
testconfdb_LDADD	= -lconfdb ../lcr/liblcr.a
testconfdb_LDFLAGS	= -L../lib
testquorum_LDADD	= -lquorum
testquorum_LDFLAGS	= -L../lib
testvotequorum1_LDADD	= -lvotequorum
testvotequorum1_LDFLAGS	= -L../lib
testvotequorum2_LDADD	= -lvotequorum
testvotequorum2_LDFLAGS	= -L../lib
evsverify_LDADD		= -levs -ltotem_pg
evsverify_LDFLAGS	= -L../lib -L../exec
evsbench_LDADD		= -levs
evsbench_LDFLAGS	= -L../lib
cpgbench_LDADD		= -lcpg
cpgbench_LDFLAGS	= -L../lib
logsysbench_LDADD	= -llogsys
logsysbench_LDFLAGS	= -L../exec
logsysrec_LDADD		= -llogsys
logsysrec_LDFLAGS	= -L../exec

lint:
	-splint $(LINT_FLAGS) $(CFLAGS) *.c


