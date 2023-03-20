
VLOG=/tool/mentor/questa-10.7c/questasim/bin/vlog
VSIM=/tool/mentor/questa-10.7c/questasim/bin/vsim
VCOVER=/tool/mentor/questa-10.7c/questasim/bin/vcover
VOPT=/tool/mentor/questa-10.7c/questasim/bin/vopt

TEST = dma_model_base_test

QUESTA_SIM_PATH  = '/tool/mentor/questa-10.7c/questasim/bin'

compile:        
	$(VLOG) /home/thanavignesh/Documents/uvm_project_2/rtl/design.sv /home/thanavignesh/Documents/uvm_project_2/uvm_tb/src/testbench.sv -l compile.log

RUN: compile
	$(VSIM) tbench_top "+UVM_TESTNAME="dma_model_base_test +UVM_VERBOSITY=UVM_HIGH -wlf waveform.wlf -do "log -r /*" -do "run -all" -c

RUN_WAVE: RUN
	$(VSIM) waveform.wlf

####################################################################################################################

