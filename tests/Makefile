SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/wrappers/cocotb_test.v
or:
	$(MAKE) sim MODULE=cocotb_test TOPLEVEL=cocotb_test
include $(shell cocotb-config --makefiles)/Makefile.sim
