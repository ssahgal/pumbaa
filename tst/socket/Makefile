#
# @section License
#
# The MIT License (MIT)
# 
# Copyright (c) 2016-2017, Erik Moqvist
# 
# Permission is hereby granted, free of charge, to any person
# obtaining a copy of this software and associated documentation
# files (the "Software"), to deal in the Software without
# restriction, including without limitation the rights to use, copy,
# modify, merge, publish, distribute, sublicense, and/or sell copies
# of the Software, and to permit persons to whom the Software is
# furnished to do so, subject to the following conditions:
#
# The above copyright notice and this permission notice shall be
# included in all copies or substantial portions of the Software.
#
# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
# EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
# MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
# NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
# BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
# ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
# CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
# SOFTWARE.
#
# This file is part of the Pumbaa project.
#


NAME = socket_suite
TYPE = suite
BOARD ?= linux

INC += \
	$(PUMBAA_ROOT)/tst/stubs
SRC += \
	$(PUMBAA_ROOT)/tst/stubs/socket_stub.c

CDEFS += \
	CONFIG_MINIMAL_SYSTEM=1 \
	CONFIG_PUMBAA_MODULE_SOCKET=1 \
	CONFIG_PUMBAA_MODULE_SELECT=1 \
	CONFIG_FS_CMD_THRD_LIST=1 \
	CONFIG_PUMBAA_MAIN_REBOOT_AT_EXIT=0 \
	CONFIG_PUMBAA_MAIN_FRIENDLY_REPL=0

SYNC_SRC = event.c
INET_SRC = inet.c

PUMBAA_ROOT ?= ../..
include $(PUMBAA_ROOT)/make/app.mk
