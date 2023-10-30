SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/wrappers/cocotb_test.v
all: dut
dut:
	$(MAKE) sim MODULE=cocotb_test TOPLEVEL=cocctb_test
include $(shell cocotb-config --makefiles)/Makefile.sim
