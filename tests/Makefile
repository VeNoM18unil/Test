SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/wrappers/cocotb_test.v
VERILOG_SOURCES += $(PWD)/wrappers/ifc_test.v
VERILOG_SOURCES += $(PWD)/../hdl/ifc_or.v
VERILOG_SOURCES += $(PWD)/../hdl/FIFO1.v
VERILOG_SOURCES += $(PWD)/../hdl/FIFO2.v
all: or ifc
or:
	rm -rf sim_build
	$(MAKE) sim MODULE=cocotb_test TOPLEVEL=cocctb_test
ifc:
	rm -rf sim_build
	$(MAKE) sim MODULE=ifc_test TOPLEVEL=ifc_test
coverage:
	rm -rf sim_build
	$(MAKE) sim MODULE=ifc_coverage TOPLEVEL=ifc_test
include $(shell cocotb-config --makefiles)/Makefile.sim
