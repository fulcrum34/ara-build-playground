# stage-1-Synth LOG

```
synth_design -rtl -name rtl_1
Command: synth_design -rtl -name rtl_1
Starting synth_design
Using part: xczu9eg-ffvb1156-2-e
Top: ara
WARNING: [Synth 8-1921] elaboration system task fatal violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:71]
WARNING: [Synth 8-1921] elaboration system task fatal violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:79]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane.sv:457]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/popcount.sv:31]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_alu.sv:534]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_mul.sv:306]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu_op_dp.sv:16814]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:450]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:453]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:456]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:459]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:464]
WARNING: [Synth 8-1921] elaboration system task error violates IEEE 1800 syntax [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:467]
---------------------------------------------------------------------------------
Starting RTL Elaboration : Time (s): cpu = 00:00:03 ; elapsed = 00:00:03 . Memory (MB): peak = 8550.781 ; gain = 2.555 ; free physical = 558 ; free virtual = 7723
---------------------------------------------------------------------------------
INFO: [Synth 8-6157] synthesizing module 'ara' [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:9]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter FPExtSupport bound to: 1'b1 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter AxiDataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter AxiAddrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter NrPEs bound to: 32'b00000000000000000000000000000110 
	Parameter MaxVLenPerLane bound to: 32'b00000000000000000000000001000000 
	Parameter MaxVLenBPerLane bound to: 32'b00000000000000000000000000001000 
	Parameter VRFSizePerLane bound to: 32'b00000000000000000000100000000000 
	Parameter VRFBSizePerLane bound to: 32'b00000000000000000000000100000000 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'lane' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane.sv:12]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter FPExtSupport bound to: 1'b1 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter MaxVLenPerLane bound to: 32'b00000000000000000000000001000000 
	Parameter MaxVLenBPerLane bound to: 32'b00000000000000000000000000001000 
	Parameter VRFSizePerLane bound to: 32'b00000000000000000000100000000000 
	Parameter VRFBSizePerLane bound to: 32'b00000000000000000000000100000000 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
INFO: [Synth 8-6157] synthesizing module 'spill_register' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
	Parameter Bypass bound to: 1'b0 
INFO: [Synth 8-6157] synthesizing module 'spill_register_flushable' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
	Parameter Bypass bound to: 1'b0 
INFO: [Synth 8-6155] done synthesizing module 'spill_register_flushable' (1#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
INFO: [Synth 8-6155] done synthesizing module 'spill_register' (2#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
INFO: [Synth 8-6157] synthesizing module 'lane_sequencer' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:11]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
INFO: [Synth 8-6157] synthesizing module 'fall_through_register' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fall_through_register.sv:15]
INFO: [Synth 8-6157] synthesizing module 'fifo_v3' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b1 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000001 
WARNING: [Synth 8-5858] RAM mem_n_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mem_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element read_pointer_q_reg was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:116]
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3' (3#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6155] done synthesizing module 'fall_through_register' (4#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fall_through_register.sv:15]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:201]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:288]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:540]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:564]
INFO: [Synth 8-155] case statement is not full and has no default [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:598]
WARNING: [Synth 8-5858] RAM operand_request_d_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM operand_request_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM operand_request_i_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'lane_sequencer' (5#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane_sequencer.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_requester' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_requester.sv:11]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter NrBanks bound to: 32'b00000000000000000000000000001000 
	Parameter NrMasters bound to: 14 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'rr_arb_tree' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
	Parameter NumIn bound to: 32'b00000000000000000000000000000111 
	Parameter DataWidth bound to: 32'b00000000000000000000000001010101 
	Parameter ExtPrio bound to: 1'b0 
	Parameter AxiVldRdy bound to: 1'b0 
	Parameter LockIn bound to: 1'b0 
	Parameter FairArb bound to: 1'b1 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6157] synthesizing module 'lzc' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000000111 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6155] done synthesizing module 'lzc' (6#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6155] done synthesizing module 'rr_arb_tree' (7#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
INFO: [Synth 8-6157] synthesizing module 'rr_arb_tree__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
	Parameter NumIn bound to: 32'b00000000000000000000000000000010 
	Parameter DataWidth bound to: 32'b00000000000000000000000001010101 
	Parameter ExtPrio bound to: 1'b1 
	Parameter AxiVldRdy bound to: 1'b0 
	Parameter LockIn bound to: 1'b0 
	Parameter FairArb bound to: 1'b1 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000001 
INFO: [Synth 8-6155] done synthesizing module 'rr_arb_tree__parameterized0' (7#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
INFO: [Synth 8-6157] synthesizing module 'stream_register' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_register.sv:16]
INFO: [Synth 8-6155] done synthesizing module 'stream_register' (8#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_register.sv:16]
WARNING: [Synth 8-5858] RAM operand_payload_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM operand_queue_cmd_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'operand_requester' (9#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_requester.sv:11]
INFO: [Synth 8-6157] synthesizing module 'vector_regfile' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vector_regfile.sv:9]
	Parameter NrBanks bound to: 32'b00000000000000000000000000001000 
	Parameter VRFSize bound to: 32'b00000000000000000000100000000000 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter NumWords bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6157] synthesizing module 'tc_clk_gating' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/tech_cells_generic/src/rtl/tc_clk.sv:31]
	Parameter IS_FUNCTIONAL bound to: 1'b1 
INFO: [Synth 8-6155] done synthesizing module 'tc_clk_gating' (10#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/tech_cells_generic/src/rtl/tc_clk.sv:31]
INFO: [Synth 8-6157] synthesizing module 'tc_sram' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/tech_cells_generic/src/rtl/tc_sram.sv:56]
	Parameter NumWords bound to: 32'b00000000000000000000000000000100 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter ByteWidth bound to: 8 - type: integer 
	Parameter NumPorts bound to: 32'b00000000000000000000000000000001 
	Parameter Latency bound to: 1 - type: integer 
	Parameter SimInit bound to: none - type: string 
	Parameter PrintSimCfg bound to: 1'b0 
	Parameter ImplKey bound to: none - type: string 
	Parameter AddrWidth bound to: 32'b00000000000000000000000000000010 
	Parameter BeWidth bound to: 32'b00000000000000000000000000001000 
WARNING: [Synth 8-5856] 3D RAM rdata_d_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5856] 3D RAM rdata_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5788] Register rdata_q_reg[0][0] in module tc_sram is has both Set and reset with same priority. This may cause simulation mismatches. Consider rewriting code  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/tech_cells_generic/src/rtl/tc_sram.sv:140]
WARNING: [Synth 8-5788] Register sram_reg in module tc_sram is has both Set and reset with same priority. This may cause simulation mismatches. Consider rewriting code 
WARNING: [Synth 8-4767] Trying to implement RAM 'sram_reg' in registers. Block RAM or DRAM implementation is not possible; see log for reasons.
Reason is one or more of the following :
	1: RAM is sensitive to asynchronous reset signal. this RTL style is not supported. 
RAM "sram_reg" dissolved into registers
INFO: [Synth 8-6155] done synthesizing module 'tc_sram' (11#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/tech_cells_generic/src/rtl/tc_sram.sv:56]
INFO: [Synth 8-6157] synthesizing module 'stream_xbar' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_xbar.sv:16]
	Parameter NumInp bound to: 32'b00000000000000000000000000001000 
	Parameter NumOut bound to: 32'b00000000000000000000000000001001 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter OutSpillReg bound to: 1'b0 
	Parameter ExtPrio bound to: 0 - type: integer 
	Parameter AxiVldRdy bound to: -1 - type: integer 
	Parameter LockIn bound to: 1 - type: integer 
	Parameter SelWidth bound to: 32'b00000000000000000000000000000100 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6157] synthesizing module 'stream_demux' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_demux.sv:15]
	Parameter N_OUP bound to: 32'b00000000000000000000000000001001 
	Parameter LOG_N_OUP bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6155] done synthesizing module 'stream_demux' (12#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_demux.sv:15]
INFO: [Synth 8-6157] synthesizing module 'rr_arb_tree__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
	Parameter NumIn bound to: 32'b00000000000000000000000000001000 
	Parameter DataWidth bound to: 32'b00000000000000000000000000100000 
	Parameter ExtPrio bound to: 1'b0 
	Parameter AxiVldRdy bound to: 1'b1 
	Parameter LockIn bound to: 1'b1 
	Parameter FairArb bound to: 1'b1 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000001000 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized0' (12#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6155] done synthesizing module 'rr_arb_tree__parameterized1' (12#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
INFO: [Synth 8-6157] synthesizing module 'spill_register__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
	Parameter Bypass bound to: 1'b1 
INFO: [Synth 8-6157] synthesizing module 'spill_register_flushable__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
	Parameter Bypass bound to: 1'b1 
INFO: [Synth 8-6155] done synthesizing module 'spill_register_flushable__parameterized0' (12#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
INFO: [Synth 8-6155] done synthesizing module 'spill_register__parameterized0' (12#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
INFO: [Synth 8-6155] done synthesizing module 'stream_xbar' (13#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_xbar.sv:16]
INFO: [Synth 8-6155] done synthesizing module 'vector_regfile' (14#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vector_regfile.sv:9]
INFO: [Synth 8-6157] synthesizing module 'operand_queues_stage' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queues_stage.sv:9]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
INFO: [Synth 8-6157] synthesizing module 'operand_queue' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000100 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000101 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b1 
	Parameter SupportIntExt4 bound to: 1'b1 
	Parameter SupportIntExt8 bound to: 1'b1 
	Parameter SupportReduct bound to: 1'b1 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000100 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000010 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000100 
WARNING: [Synth 8-5858] RAM mem_n_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mem_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized0' (14#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000101 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000011 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000101 
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized1' (14#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:191]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:199]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:201]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:208]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:216]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:234]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:254]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:257]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:268]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:277]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:286]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:297]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:306]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:316]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:331]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:361]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:416]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:434]
INFO: [Synth 8-6155] done synthesizing module 'operand_queue' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000100 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000101 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b1 
	Parameter SupportIntExt4 bound to: 1'b1 
	Parameter SupportIntExt8 bound to: 1'b1 
	Parameter SupportReduct bound to: 1'b1 
	Parameter SupportNtrVal bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:191]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:199]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:201]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:208]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:216]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:234]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:254]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:257]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:268]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:277]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:286]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:297]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:306]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:316]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:331]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:361]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:373]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:416]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:434]
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized0' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000100 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000101 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b1 
	Parameter SupportIntExt4 bound to: 1'b0 
	Parameter SupportIntExt8 bound to: 1'b0 
	Parameter SupportReduct bound to: 1'b1 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:191]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:199]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:201]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:208]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:216]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:234]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:254]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:257]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:286]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:316]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:331]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:361]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:416]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:434]
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized1' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000100 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000101 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b1 
	Parameter SupportIntExt4 bound to: 1'b0 
	Parameter SupportIntExt8 bound to: 1'b0 
	Parameter SupportReduct bound to: 1'b1 
	Parameter SupportNtrVal bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:454]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:189]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:191]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:199]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:201]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:208]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:216]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:234]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:254]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:257]
INFO: [Synth 8-294] found qualifier unique on case statement: implementing as parallel_case [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:286]
INFO: [Common 17-14] Message 'Synth 8-294' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized2' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized3' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000101 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000010 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b0 
	Parameter SupportIntExt4 bound to: 1'b0 
	Parameter SupportIntExt8 bound to: 1'b0 
	Parameter SupportReduct bound to: 1'b0 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000101 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000011 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000101 
WARNING: [Synth 8-5858] RAM mem_n_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mem_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized2' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized3' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000010 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000010 
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized3' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized3' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized4' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000100 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000010 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b0 
	Parameter SupportIntExt4 bound to: 1'b0 
	Parameter SupportIntExt8 bound to: 1'b0 
	Parameter SupportReduct bound to: 1'b0 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized4' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized5' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000001 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000001 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b1 
	Parameter SupportIntExt4 bound to: 1'b1 
	Parameter SupportIntExt8 bound to: 1'b1 
	Parameter SupportReduct bound to: 1'b0 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized4' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000001 
WARNING: [Synth 8-5858] RAM mem_n_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mem_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element read_pointer_q_reg was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:116]
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized4' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6157] synthesizing module 'fifo_v3__parameterized5' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
	Parameter FALL_THROUGH bound to: 1'b0 
	Parameter DATA_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter ADDR_DEPTH bound to: 32'b00000000000000000000000000000001 
	Parameter FifoDepth bound to: 32'b00000000000000000000000000000001 
WARNING: [Synth 8-6014] Unused sequential element read_pointer_q_reg was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:116]
INFO: [Synth 8-6155] done synthesizing module 'fifo_v3__parameterized5' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/fifo_v3.sv:13]
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized5' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6157] synthesizing module 'operand_queue__parameterized6' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
	Parameter CmdBufDepth bound to: 32'b00000000000000000000000000000001 
	Parameter DataBufDepth bound to: 32'b00000000000000000000000000000001 
	Parameter NrSlaves bound to: 32'b00000000000000000000000000000001 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter SupportIntExt2 bound to: 1'b0 
	Parameter SupportIntExt4 bound to: 1'b0 
	Parameter SupportIntExt8 bound to: 1'b0 
	Parameter SupportReduct bound to: 1'b0 
	Parameter SupportNtrVal bound to: 1'b0 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6155] done synthesizing module 'operand_queue__parameterized6' (15#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queue.sv:11]
INFO: [Synth 8-6155] done synthesizing module 'operand_queues_stage' (16#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/operand_queues_stage.sv:9]
INFO: [Synth 8-6157] synthesizing module 'vector_fus_stage' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vector_fus_stage.sv:10]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter FPExtSupport bound to: 1'b1 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
INFO: [Synth 8-6157] synthesizing module 'valu' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:10]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter VInsnQueueDepth bound to: 4 - type: integer 
	Parameter ResultQueueDepth bound to: 32'b00000000000000000000000000000010 
INFO: [Synth 8-6157] synthesizing module 'fixed_p_rounding' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/fixed_p_rounding.sv:9]
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6155] done synthesizing module 'fixed_p_rounding' (17#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/fixed_p_rounding.sv:9]
INFO: [Synth 8-6157] synthesizing module 'stream_register__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_register.sv:16]
INFO: [Synth 8-6155] done synthesizing module 'stream_register__parameterized0' (17#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/stream_register.sv:16]
INFO: [Synth 8-6157] synthesizing module 'spill_register__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
	Parameter Bypass bound to: 1'b0 
INFO: [Synth 8-6157] synthesizing module 'spill_register_flushable__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
	Parameter Bypass bound to: 1'b0 
INFO: [Synth 8-6155] done synthesizing module 'spill_register_flushable__parameterized1' (17#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register_flushable.sv:17]
INFO: [Synth 8-6155] done synthesizing module 'spill_register__parameterized1' (17#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/spill_register.sv:17]
INFO: [Synth 8-6157] synthesizing module 'simd_alu' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_alu.sv:9]
	Parameter FixPtSupport bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6155] done synthesizing module 'simd_alu' (18#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_alu.sv:9]
WARNING: [Synth 8-5858] RAM result_queue_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM result_queue_d_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][3][vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][2][vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][0][vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:100]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:117]
INFO: [Synth 8-6155] done synthesizing module 'valu' (19#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/valu.sv:10]
INFO: [Synth 8-6157] synthesizing module 'vmfpu' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vmfpu.sv:10]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter FPExtSupport bound to: 1'b1 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter VInsnQueueDepth bound to: 4 - type: integer 
	Parameter ResultQueueDepth bound to: 32'b00000000000000000000000000000010 
INFO: [Synth 8-6157] synthesizing module 'power_gating_generic' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/power_gating_generic.sv:9]
	Parameter NO_GLITCH bound to: 0 - type: integer 
INFO: [Synth 8-6155] done synthesizing module 'power_gating_generic' (20#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/power_gating_generic.sv:9]
INFO: [Synth 8-6157] synthesizing module 'power_gating_generic__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/power_gating_generic.sv:9]
	Parameter NO_GLITCH bound to: 0 - type: integer 
INFO: [Synth 8-6155] done synthesizing module 'power_gating_generic__parameterized0' (20#1) [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/power_gating_generic.sv:9]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000001010 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized1' (20#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000010111 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000101 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized2' (20#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized3' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000110100 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000110 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized3' (20#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'fpnew_top' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_top.sv:16]
	Parameter Features[Width] bound to: 64 - type: integer 
	Parameter Features[EnableVectors] bound to: 1'b1 
	Parameter Features[EnableNanBox] bound to: 1'b1 
	Parameter Features[FpFmtMask] bound to: 6'b111000 
	Parameter Features[IntFmtMask] bound to: 4'b0111 
	Parameter Implementation[PipeRegs][0][0] bound to: 4 - type: integer 
	Parameter Implementation[PipeRegs][0][1] bound to: 5 - type: integer 
	Parameter Implementation[PipeRegs][0][2] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][0][3] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][0][4] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][0][5] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][1][0] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][1][1] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][1][2] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][1][3] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][1][4] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][1][5] bound to: 3 - type: integer 
	Parameter Implementation[PipeRegs][2][0] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][2][1] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][2][2] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][2][3] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][2][4] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][2][5] bound to: 1 - type: integer 
	Parameter Implementation[PipeRegs][3][0] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][3][1] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][3][2] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][3][3] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][3][4] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][3][5] bound to: 2 - type: integer 
	Parameter Implementation[PipeRegs][4][0] bound to: 0 - type: integer 
	Parameter Implementation[PipeRegs][4][1] bound to: 0 - type: integer 
	Parameter Implementation[PipeRegs][4][2] bound to: 0 - type: integer 
	Parameter Implementation[PipeRegs][4][3] bound to: 0 - type: integer 
	Parameter Implementation[PipeRegs][4][4] bound to: 0 - type: integer 
	Parameter Implementation[PipeRegs][4][5] bound to: 0 - type: integer 
	Parameter Implementation[UnitTypes][0][0] bound to: 2'b01 
	Parameter Implementation[UnitTypes][0][1] bound to: 2'b01 
	Parameter Implementation[UnitTypes][0][2] bound to: 2'b01 
	Parameter Implementation[UnitTypes][0][3] bound to: 2'b01 
	Parameter Implementation[UnitTypes][0][4] bound to: 2'b01 
	Parameter Implementation[UnitTypes][0][5] bound to: 2'b01 
	Parameter Implementation[UnitTypes][1][0] bound to: 2'b10 
	Parameter Implementation[UnitTypes][1][1] bound to: 2'b10 
	Parameter Implementation[UnitTypes][1][2] bound to: 2'b10 
	Parameter Implementation[UnitTypes][1][3] bound to: 2'b10 
	Parameter Implementation[UnitTypes][1][4] bound to: 2'b10 
	Parameter Implementation[UnitTypes][1][5] bound to: 2'b10 
	Parameter Implementation[UnitTypes][2][0] bound to: 2'b01 
	Parameter Implementation[UnitTypes][2][1] bound to: 2'b01 
	Parameter Implementation[UnitTypes][2][2] bound to: 2'b01 
	Parameter Implementation[UnitTypes][2][3] bound to: 2'b01 
	Parameter Implementation[UnitTypes][2][4] bound to: 2'b01 
	Parameter Implementation[UnitTypes][2][5] bound to: 2'b01 
	Parameter Implementation[UnitTypes][3][0] bound to: 2'b10 
	Parameter Implementation[UnitTypes][3][1] bound to: 2'b10 
	Parameter Implementation[UnitTypes][3][2] bound to: 2'b10 
	Parameter Implementation[UnitTypes][3][3] bound to: 2'b10 
	Parameter Implementation[UnitTypes][3][4] bound to: 2'b10 
	Parameter Implementation[UnitTypes][3][5] bound to: 2'b10 
	Parameter Implementation[UnitTypes][4][0] bound to: 2'b00 
	Parameter Implementation[UnitTypes][4][1] bound to: 2'b00 
	Parameter Implementation[UnitTypes][4][2] bound to: 2'b00 
	Parameter Implementation[UnitTypes][4][3] bound to: 2'b00 
	Parameter Implementation[UnitTypes][4][4] bound to: 2'b00 
	Parameter Implementation[UnitTypes][4][5] bound to: 2'b00 
	Parameter Implementation[PipeConfig] bound to: 2'b11 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter EnableSIMDMask bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NumLanes bound to: 32'b00000000000000000000000000000100 
	Parameter WIDTH bound to: 64 - type: integer 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_OPGROUPS bound to: 32'b00000000000000000000000000000101 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_block' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter OpGroup bound to: 3'b000 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter FpFmtMask bound to: 6'b111000 
	Parameter IntFmtMask bound to: 4'b0111 
	Parameter FmtPipeRegs bound to: 192'b000000000000000000000000000001000000000000000000000000000000010100000000000000000000000000000011000000000000000000000000000000100000000000000000000000000000001100000000000000000000000000000010 
	Parameter FmtUnitTypes bound to: 12'b010101010101 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b000 
	Parameter FpFormat bound to: 3'b000 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 4 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000010 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000010000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_fma' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
	Parameter FpFormat bound to: 3'b000 
	Parameter NumPipeRegs bound to: 4 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter EXP_BITS bound to: 8 - type: integer 
	Parameter MAN_BITS bound to: 23 - type: integer 
	Parameter BIAS bound to: 32'b00000000000000000000000001111111 
	Parameter PRECISION_BITS bound to: 32'b00000000000000000000000000011000 
	Parameter LOWER_SUM_WIDTH bound to: 32'b00000000000000000000000000110011 
	Parameter LZC_RESULT_WIDTH bound to: 32'b00000000000000000000000000000110 
	Parameter EXP_WIDTH bound to: 32'b00000000000000000000000000001010 
	Parameter SHIFT_AMOUNT_WIDTH bound to: 32'b00000000000000000000000000000111 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_MID_REGS bound to: 2 - type: integer 
	Parameter NUM_OUT_REGS bound to: 1 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b000 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000011 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter EXP_BITS bound to: 8 - type: integer 
	Parameter MAN_BITS bound to: 23 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier' (21#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized4' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000110011 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000110 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized4' (21#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'fpnew_rounding' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
	Parameter AbsWidth bound to: 32'b00000000000000000000000000011111 
	Parameter EnableRSR bound to: 1'b0 
	Parameter RsrPrecision bound to: 32'b00000000000000000000000000001100 
	Parameter LfsrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter RstVal bound to: -1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:83]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_rounding' (22#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_res_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_stat_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_result_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-3936] Found unconnected internal register 'final_mantissa_reg' and it is trimmed from '25' to '24' bits. [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:546]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_fma' (23#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b000 
	Parameter FpFormat bound to: 3'b001 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 5 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000001 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_fma__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
	Parameter FpFormat bound to: 3'b001 
	Parameter NumPipeRegs bound to: 5 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter EXP_BITS bound to: 11 - type: integer 
	Parameter MAN_BITS bound to: 52 - type: integer 
	Parameter BIAS bound to: 32'b00000000000000000000001111111111 
	Parameter PRECISION_BITS bound to: 32'b00000000000000000000000000110101 
	Parameter LOWER_SUM_WIDTH bound to: 32'b00000000000000000000000001101101 
	Parameter LZC_RESULT_WIDTH bound to: 32'b00000000000000000000000000000111 
	Parameter EXP_WIDTH bound to: 32'b00000000000000000000000000001101 
	Parameter SHIFT_AMOUNT_WIDTH bound to: 32'b00000000000000000000000000001000 
	Parameter NUM_INP_REGS bound to: 2 - type: integer 
	Parameter NUM_MID_REGS bound to: 2 - type: integer 
	Parameter NUM_OUT_REGS bound to: 1 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b001 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000011 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter EXP_BITS bound to: 11 - type: integer 
	Parameter MAN_BITS bound to: 52 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized0' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized5' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000001101101 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000111 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized5' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'fpnew_rounding__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
	Parameter AbsWidth bound to: 32'b00000000000000000000000000111111 
	Parameter EnableRSR bound to: 1'b0 
	Parameter RsrPrecision bound to: 32'b00000000000000000000000000001100 
	Parameter LfsrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter RstVal bound to: -1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:83]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_rounding__parameterized0' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_res_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_stat_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_result_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-3936] Found unconnected internal register 'final_mantissa_reg' and it is trimmed from '54' to '53' bits. [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:546]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_fma__parameterized0' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice__parameterized0' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b000 
	Parameter FpFormat bound to: 3'b010 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 3 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000100000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_fma__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
	Parameter FpFormat bound to: 3'b010 
	Parameter NumPipeRegs bound to: 3 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter EXP_BITS bound to: 5 - type: integer 
	Parameter MAN_BITS bound to: 10 - type: integer 
	Parameter BIAS bound to: 32'b00000000000000000000000000001111 
	Parameter PRECISION_BITS bound to: 32'b00000000000000000000000000001011 
	Parameter LOWER_SUM_WIDTH bound to: 32'b00000000000000000000000000011001 
	Parameter LZC_RESULT_WIDTH bound to: 32'b00000000000000000000000000000101 
	Parameter EXP_WIDTH bound to: 32'b00000000000000000000000000000111 
	Parameter SHIFT_AMOUNT_WIDTH bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_MID_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 1 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b010 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000011 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter EXP_BITS bound to: 5 - type: integer 
	Parameter MAN_BITS bound to: 10 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized1' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized6' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000011001 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000101 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized6' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6157] synthesizing module 'fpnew_rounding__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
	Parameter AbsWidth bound to: 32'b00000000000000000000000000001111 
	Parameter EnableRSR bound to: 1'b0 
	Parameter RsrPrecision bound to: 32'b00000000000000000000000000001100 
	Parameter LfsrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter RstVal bound to: -1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:83]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_rounding__parameterized1' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_res_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM mid_pipe_spec_stat_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_result_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-3936] Found unconnected internal register 'final_mantissa_reg' and it is trimmed from '12' to '11' bits. [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:546]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_fma__parameterized1' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_fma.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice__parameterized1' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6157] synthesizing module 'rr_arb_tree__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
	Parameter NumIn bound to: 32'b00000000000000000000000000000110 
	Parameter DataWidth bound to: 32'b00000000000000000000000000100000 
	Parameter ExtPrio bound to: 1'b0 
	Parameter AxiVldRdy bound to: 1'b1 
	Parameter LockIn bound to: 1'b0 
	Parameter FairArb bound to: 1'b1 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized7' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000000110 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized7' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6155] done synthesizing module 'rr_arb_tree__parameterized2' (24#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_block' (25#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_block__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter OpGroup bound to: 3'b001 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter FpFmtMask bound to: 6'b111000 
	Parameter IntFmtMask bound to: 4'b0111 
	Parameter FmtPipeRegs bound to: 192'b000000000000000000000000000000110000000000000000000000000000001100000000000000000000000000000011000000000000000000000000000000110000000000000000000000000000001100000000000000000000000000000011 
	Parameter FmtUnitTypes bound to: 12'b101010101010 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_multifmt_slice' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:18]
	Parameter OpGroup bound to: 3'b001 
	Parameter Width bound to: 64 - type: integer 
	Parameter FpFmtConfig bound to: 6'b111000 
	Parameter IntFmtConfig bound to: 4'b0111 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000011 
	Parameter PipeConfig bound to: 2'b11 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_SIMD_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter MAX_FP_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter MAX_INT_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter NUM_DOTP_LANES bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_INT_FORMATS bound to: 32'b00000000000000000000000000000100 
	Parameter FMT_BITS bound to: 32'b00000000000000000000000000000011 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000111 
INFO: [Synth 8-6157] synthesizing module 'fpnew_divsqrt_multi' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
	Parameter FpFmtConfig bound to: 6'b111000 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000011 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 2 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'div_sqrt_top_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/div_sqrt_top_mvp.sv:37]
INFO: [Synth 8-6157] synthesizing module 'preprocess_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/preprocess_mvp.sv:37]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized8' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000000110101 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000110 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized8' (25#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6155] done synthesizing module 'preprocess_mvp' (26#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/preprocess_mvp.sv:37]
INFO: [Synth 8-6157] synthesizing module 'nrbd_nrsc_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/nrbd_nrsc_mvp.sv:36]
INFO: [Synth 8-6157] synthesizing module 'control_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/control_mvp.sv:43]
INFO: [Synth 8-6157] synthesizing module 'iteration_div_sqrt_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/iteration_div_sqrt_mvp.sv:32]
	Parameter WIDTH bound to: 58 - type: integer 
INFO: [Synth 8-6155] done synthesizing module 'iteration_div_sqrt_mvp' (27#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/iteration_div_sqrt_mvp.sv:32]
WARNING: [Synth 8-3848] Net Iteration_cell_sum_AMASK_D[3] in module/entity control_mvp does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/control_mvp.sv:842]
WARNING: [Synth 8-3848] Net Iteration_cell_carry_D[3] in module/entity control_mvp does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/control_mvp.sv:840]
INFO: [Synth 8-6155] done synthesizing module 'control_mvp' (28#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/control_mvp.sv:43]
INFO: [Synth 8-6155] done synthesizing module 'nrbd_nrsc_mvp' (29#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/nrbd_nrsc_mvp.sv:36]
INFO: [Synth 8-6157] synthesizing module 'norm_div_sqrt_mvp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/norm_div_sqrt_mvp.sv:46]
INFO: [Synth 8-6155] done synthesizing module 'norm_div_sqrt_mvp' (30#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/norm_div_sqrt_mvp.sv:46]
INFO: [Synth 8-6155] done synthesizing module 'div_sqrt_top_mvp' (31#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpu_div_sqrt_mvp/hdl/div_sqrt_top_mvp.sv:37]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_divsqrt_multi' (32#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
INFO: [Synth 8-6157] synthesizing module 'fpnew_divsqrt_multi__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
	Parameter FpFmtConfig bound to: 6'b101000 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000011 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 2 - type: integer 
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_divsqrt_multi__parameterized0' (32#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
INFO: [Synth 8-6157] synthesizing module 'fpnew_divsqrt_multi__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
	Parameter FpFmtConfig bound to: 6'b001000 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000011 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 2 - type: integer 
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM out_pipe_status_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_divsqrt_multi__parameterized1' (32#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_divsqrt_multi.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_multifmt_slice' (33#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_block__parameterized0' (33#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_block__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter OpGroup bound to: 3'b010 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter FpFmtMask bound to: 6'b111000 
	Parameter IntFmtMask bound to: 4'b0111 
	Parameter FmtPipeRegs bound to: 192'b000000000000000000000000000000010000000000000000000000000000000100000000000000000000000000000001000000000000000000000000000000010000000000000000000000000000000100000000000000000000000000000001 
	Parameter FmtUnitTypes bound to: 12'b010101010101 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b010 
	Parameter FpFormat bound to: 3'b000 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000010 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000010000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_noncomp' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
	Parameter FpFormat bound to: 3'b000 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter EXP_BITS bound to: 8 - type: integer 
	Parameter MAN_BITS bound to: 23 - type: integer 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 0 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b000 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000010 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter EXP_BITS bound to: 8 - type: integer 
	Parameter MAN_BITS bound to: 23 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized2' (33#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_noncomp' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice__parameterized2' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice__parameterized3' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b010 
	Parameter FpFormat bound to: 3'b001 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000001 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_noncomp__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
	Parameter FpFormat bound to: 3'b001 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter EXP_BITS bound to: 11 - type: integer 
	Parameter MAN_BITS bound to: 52 - type: integer 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 0 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized3' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b001 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000010 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter EXP_BITS bound to: 11 - type: integer 
	Parameter MAN_BITS bound to: 52 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized3' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_noncomp__parameterized0' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice__parameterized3' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_fmt_slice__parameterized4' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
	Parameter OpGroup bound to: 3'b010 
	Parameter FpFormat bound to: 3'b010 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter FP_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter SIMD_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000010 
	Parameter CLASS_VEC_BITS bound to: 32'b00000000000000000000000000100000 
INFO: [Synth 8-6157] synthesizing module 'fpnew_noncomp__parameterized1' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
	Parameter FpFormat bound to: 3'b010 
	Parameter NumPipeRegs bound to: 1 - type: integer 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter EXP_BITS bound to: 5 - type: integer 
	Parameter MAN_BITS bound to: 10 - type: integer 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 0 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized4' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b010 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000010 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter EXP_BITS bound to: 5 - type: integer 
	Parameter MAN_BITS bound to: 10 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized4' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
WARNING: [Synth 8-5856] 3D RAM inp_pipe_operands_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_noncomp__parameterized1' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_noncomp.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_fmt_slice__parameterized4' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_fmt_slice.sv:16]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_block__parameterized1' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_block__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter OpGroup bound to: 3'b011 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter FpFmtMask bound to: 6'b111000 
	Parameter IntFmtMask bound to: 4'b0111 
	Parameter FmtPipeRegs bound to: 192'b000000000000000000000000000000100000000000000000000000000000001000000000000000000000000000000010000000000000000000000000000000100000000000000000000000000000001000000000000000000000000000000010 
	Parameter FmtUnitTypes bound to: 12'b101010101010 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6157] synthesizing module 'fpnew_opgroup_multifmt_slice__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:18]
	Parameter OpGroup bound to: 3'b011 
	Parameter Width bound to: 64 - type: integer 
	Parameter FpFmtConfig bound to: 6'b111000 
	Parameter IntFmtConfig bound to: 4'b0111 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000010 
	Parameter PipeConfig bound to: 2'b11 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_SIMD_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter MAX_FP_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter MAX_INT_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
	Parameter NUM_DOTP_LANES bound to: 32'b00000000000000000000000000000010 
	Parameter NUM_INT_FORMATS bound to: 32'b00000000000000000000000000000100 
	Parameter FMT_BITS bound to: 32'b00000000000000000000000000000011 
	Parameter AUX_BITS bound to: 32'b00000000000000000000000000000111 
INFO: [Synth 8-6157] synthesizing module 'fpnew_cast_multi' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:18]
	Parameter FpFmtConfig bound to: 6'b111000 
	Parameter IntFmtConfig bound to: 4'b0111 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000010 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INT_FORMATS bound to: 32'b00000000000000000000000000000100 
	Parameter MAX_INT_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter SUPER_FORMAT[exp_bits] bound to: 11 - type: integer 
	Parameter SUPER_FORMAT[man_bits] bound to: 52 - type: integer 
	Parameter SUPER_EXP_BITS bound to: 11 - type: integer 
	Parameter SUPER_MAN_BITS bound to: 52 - type: integer 
	Parameter SUPER_BIAS bound to: 32'b00000000000000000000001111111111 
	Parameter INT_MAN_WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter LZC_RESULT_WIDTH bound to: 32'b00000000000000000000000000000110 
	Parameter INT_EXP_WIDTH bound to: 32'b00000000000000000000000000001100 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_MID_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 0 - type: integer 
	Parameter NUM_FP_STICKY bound to: 75 - type: integer 
	Parameter NUM_INT_STICKY bound to: 64 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized5' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b000 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000001 
	Parameter WIDTH bound to: 32'b00000000000000000000000000100000 
	Parameter EXP_BITS bound to: 8 - type: integer 
	Parameter MAN_BITS bound to: 23 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized5' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized6' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b001 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000001 
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter EXP_BITS bound to: 11 - type: integer 
	Parameter MAN_BITS bound to: 52 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized6' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'fpnew_classifier__parameterized7' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
	Parameter FpFormat bound to: 3'b010 
	Parameter NumOperands bound to: 32'b00000000000000000000000000000001 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter EXP_BITS bound to: 5 - type: integer 
	Parameter MAN_BITS bound to: 10 - type: integer 
WARNING: [Synth 8-5858] RAM info_o_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_classifier__parameterized7' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_classifier.sv:16]
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized9' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
	Parameter WIDTH bound to: 32'b00000000000000000000000001000000 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000110 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized9' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-6157] synthesizing module 'fpnew_rounding__parameterized2' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
	Parameter AbsWidth bound to: 32'b00000000000000000000000001000000 
	Parameter EnableRSR bound to: 1'b0 
	Parameter RsrPrecision bound to: 32'b00000000000000000000000000001100 
	Parameter LfsrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter RstVal bound to: -1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:83]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_rounding__parameterized2' (34#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
WARNING: [Synth 8-5858] RAM mid_pipe_info_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_normal] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_subnormal] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_quiet] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_src_fmt_q_reg[1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:388]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_cast_multi' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:18]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-6157] synthesizing module 'fpnew_cast_multi__parameterized0' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:18]
	Parameter FpFmtConfig bound to: 6'b001000 
	Parameter IntFmtConfig bound to: 4'b0100 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000010 
	Parameter PipeConfig bound to: 2'b11 
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INT_FORMATS bound to: 32'b00000000000000000000000000000100 
	Parameter MAX_INT_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter SUPER_FORMAT[exp_bits] bound to: 5 - type: integer 
	Parameter SUPER_FORMAT[man_bits] bound to: 10 - type: integer 
	Parameter SUPER_EXP_BITS bound to: 5 - type: integer 
	Parameter SUPER_MAN_BITS bound to: 10 - type: integer 
	Parameter SUPER_BIAS bound to: 32'b00000000000000000000000000001111 
	Parameter INT_MAN_WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter LZC_RESULT_WIDTH bound to: 32'b00000000000000000000000000000100 
	Parameter INT_EXP_WIDTH bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_INP_REGS bound to: 1 - type: integer 
	Parameter NUM_MID_REGS bound to: 1 - type: integer 
	Parameter NUM_OUT_REGS bound to: 0 - type: integer 
	Parameter NUM_FP_STICKY bound to: 21 - type: integer 
	Parameter NUM_INT_STICKY bound to: 16 - type: integer 
INFO: [Synth 8-6157] synthesizing module 'lzc__parameterized10' [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Common 17-14] Message 'Synth 8-6157' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
	Parameter WIDTH bound to: 32'b00000000000000000000000000010000 
	Parameter MODE bound to: 1'b1 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized10' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
	Parameter AbsWidth bound to: 32'b00000000000000000000000000010000 
	Parameter EnableRSR bound to: 1'b0 
	Parameter RsrPrecision bound to: 32'b00000000000000000000000000001100 
	Parameter LfsrWidth bound to: 32'b00000000000000000000000000100000 
	Parameter RstVal bound to: -1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:83]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_rounding__parameterized3' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_rounding.sv:16]
WARNING: [Synth 8-5858] RAM mid_pipe_info_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_normal] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_subnormal] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_info_q_reg[1][is_quiet] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:384]
WARNING: [Synth 8-6014] Unused sequential element gen_inside_pipeline[0].mid_pipe_src_fmt_q_reg[1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:388]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_cast_multi__parameterized0' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_cast_multi.sv:18]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_pkg.sv:95]
WARNING: [Synth 8-5856] 3D RAM fmt_conv_cpk_result_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_multifmt_slice__parameterized0' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_multifmt_slice.sv:18]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_block__parameterized2' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter OpGroup bound to: 3'b100 
	Parameter Width bound to: 64 - type: integer 
	Parameter EnableVectors bound to: 1'b1 
	Parameter PulpDivsqrt bound to: 1'b1 
	Parameter FpFmtMask bound to: 6'b111000 
	Parameter IntFmtMask bound to: 4'b0111 
	Parameter FmtPipeRegs bound to: 192'b000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000 
	Parameter FmtUnitTypes bound to: 12'b000000000000 
	Parameter PipeConfig bound to: 2'b11 
	Parameter TrueSIMDClass bound to: 1'b1 
	Parameter CompressedVecCmpResult bound to: 1'b0 
	Parameter StochasticRndImplementation[EnableRSR] bound to: 1'b0 
	Parameter StochasticRndImplementation[RsrPrecision] bound to: 12 - type: integer 
	Parameter StochasticRndImplementation[LfsrInternalPrecision] bound to: 32 - type: integer 
	Parameter NUM_FORMATS bound to: 32'b00000000000000000000000000000110 
	Parameter NUM_OPERANDS bound to: 32'b00000000000000000000000000000011 
	Parameter NUM_LANES bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-6155] done synthesizing module 'fpnew_opgroup_block__parameterized3' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_opgroup_block.sv:16]
	Parameter NumIn bound to: 32'b00000000000000000000000000000101 
	Parameter DataWidth bound to: 32'b00000000000000000000000000100000 
	Parameter ExtPrio bound to: 1'b0 
	Parameter AxiVldRdy bound to: 1'b1 
	Parameter LockIn bound to: 1'b0 
	Parameter FairArb bound to: 1'b1 
	Parameter IdxWidth bound to: 32'b00000000000000000000000000000011 
	Parameter WIDTH bound to: 32'b00000000000000000000000000000101 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000011 
INFO: [Synth 8-6155] done synthesizing module 'lzc__parameterized11' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/lzc.sv:15]
INFO: [Synth 8-6155] done synthesizing module 'rr_arb_tree__parameterized3' (35#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/common_cells/src/rr_arb_tree.sv:47]
INFO: [Synth 8-6155] done synthesizing module 'fpnew_top' (36#1) [/home/aitesam/Documents/GitHub/ara-build-playground/deps/cva6/vendor/openhwgroup/cvfpu/src/fpnew_top.sv:16]
INFO: [Common 17-14] Message 'Synth 8-6155' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1330]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1414]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1421]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1330]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1414]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1421]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1330]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1414]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1421]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1330]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1414]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1421]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1455]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1540]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1546]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1455]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1540]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1546]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1580]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1175]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1665]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1671]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/include/ara_pkg.sv:1688]
	Parameter FixPtSupport bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000001 
	Parameter ElementWidth bound to: 3'b011 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
WARNING: [Synth 8-87] always_comb on 'gen_p_mul_ew64.r_reg' did not result in combinational logic [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_mul.sv:173]
	Parameter FixPtSupport bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000001 
	Parameter ElementWidth bound to: 3'b010 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
WARNING: [Synth 8-87] always_comb on 'gen_p_mul_ew32.r_reg' did not result in combinational logic [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_mul.sv:212]
	Parameter FixPtSupport bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000001 
	Parameter ElementWidth bound to: 3'b001 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
WARNING: [Synth 8-87] always_comb on 'gen_p_mul_ew16.r_reg' did not result in combinational logic [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_mul.sv:249]
	Parameter FixPtSupport bound to: 1'b1 
	Parameter NumPipeRegs bound to: 32'b00000000000000000000000000000000 
	Parameter ElementWidth bound to: 3'b000 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_div.sv:170]
INFO: [Synth 8-155] case statement is not full and has no default [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/simd_div.sv:222]
	Parameter CVA6Cfg[NrCommitPorts] bound to: 0 - type: integer 
	Parameter CVA6Cfg[AxiAddrWidth] bound to: 0 - type: integer 
	Parameter CVA6Cfg[AxiDataWidth] bound to: 0 - type: integer 
	Parameter CVA6Cfg[AxiIdWidth] bound to: 0 - type: integer 
	Parameter CVA6Cfg[AxiUserWidth] bound to: 0 - type: integer 
	Parameter CVA6Cfg[NrLoadBufEntries] bound to: 0 - type: integer 
	Parameter CVA6Cfg[FpuEn] bound to: 1'b0 
	Parameter CVA6Cfg[XF16] bound to: 1'b0 
	Parameter CVA6Cfg[XF16ALT] bound to: 1'b0 
	Parameter CVA6Cfg[XF8] bound to: 1'b0 
	Parameter CVA6Cfg[XF8ALT] bound to: 1'b0 
	Parameter CVA6Cfg[RVA] bound to: 1'b0 
	Parameter CVA6Cfg[RVB] bound to: 1'b0 
	Parameter CVA6Cfg[RVV] bound to: 1'b0 
	Parameter CVA6Cfg[RVC] bound to: 1'b0 
	Parameter CVA6Cfg[RVH] bound to: 1'b0 
	Parameter CVA6Cfg[RVZCB] bound to: 1'b0 
	Parameter CVA6Cfg[XFVec] bound to: 1'b0 
	Parameter CVA6Cfg[CvxifEn] bound to: 1'b0 
	Parameter CVA6Cfg[ZiCondExtEn] bound to: 1'b0 
	Parameter CVA6Cfg[RVSCLIC] bound to: 1'b0 
	Parameter CVA6Cfg[RVF] bound to: 1'b0 
	Parameter CVA6Cfg[RVD] bound to: 1'b0 
	Parameter CVA6Cfg[FpPresent] bound to: 1'b0 
	Parameter CVA6Cfg[NSX] bound to: 1'b0 
	Parameter CVA6Cfg[FLen] bound to: 0 - type: integer 
	Parameter CVA6Cfg[RVFVec] bound to: 1'b0 
	Parameter CVA6Cfg[XF16Vec] bound to: 1'b0 
	Parameter CVA6Cfg[XF16ALTVec] bound to: 1'b0 
	Parameter CVA6Cfg[XF8Vec] bound to: 1'b0 
	Parameter CVA6Cfg[NrRgprPorts] bound to: 0 - type: integer 
	Parameter CVA6Cfg[NrWbPorts] bound to: 0 - type: integer 
	Parameter CVA6Cfg[EnableAccelerator] bound to: 1'b0 
	Parameter CVA6Cfg[RVS] bound to: 1'b0 
	Parameter CVA6Cfg[RVU] bound to: 1'b0 
	Parameter CVA6Cfg[HaltAddress] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExceptionAddress] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[RASDepth] bound to: 0 - type: integer 
	Parameter CVA6Cfg[BTBEntries] bound to: 0 - type: integer 
	Parameter CVA6Cfg[BHTEntries] bound to: 0 - type: integer 
	Parameter CVA6Cfg[DmBaseAddress] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[TvalEn] bound to: 1'b0 
	Parameter CVA6Cfg[NrPMPEntries] bound to: 0 - type: integer 
	Parameter CVA6Cfg[PMPCfgRstVal][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPCfgRstVal][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPAddrRstVal][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[PMPEntryReadOnly] bound to: 16'b0000000000000000 
	Parameter CVA6Cfg[NOCType] bound to: 0 - type: integer 
	Parameter CVA6Cfg[CLICNumInterruptSrc] bound to: 0 - type: integer 
	Parameter CVA6Cfg[NrNonIdempotentRules] bound to: 0 - type: integer 
	Parameter CVA6Cfg[NonIdempotentAddrBase][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentAddrBase][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NonIdempotentLength][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NrExecuteRegionRules] bound to: 0 - type: integer 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionAddrBase][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[ExecuteRegionLength][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[NrCachedRegionRules] bound to: 0 - type: integer 
	Parameter CVA6Cfg[CachedRegionAddrBase][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionAddrBase][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][15] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][14] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][13] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][12] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][11] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][10] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][9] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][8] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][7] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][6] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][5] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][4] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][3] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][2] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][1] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[CachedRegionLength][0] bound to: 64'b0000000000000000000000000000000000000000000000000000000000000000 
	Parameter CVA6Cfg[MaxOutstandingStores] bound to: 0 - type: integer 
	Parameter CVA6Cfg[DebugEn] bound to: 1'b0 
	Parameter CVA6Cfg[NonIdemPotenceEn] bound to: 1'b0 
	Parameter CVA6Cfg[AxiBurstWriteEn] bound to: 1'b0 
	Parameter WIDTH bound to: 64 - type: integer 
	Parameter STABLE_HANDSHAKE bound to: 1 - type: integer 
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vmfpu.sv:1372]
WARNING: [Synth 8-5858] RAM vfrec7_out_e16_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM vfrec7_out_e32_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM vfrec7_out_e64_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM vfrsqrt7_out_e16_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM vfrsqrt7_out_e32_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM vfrsqrt7_out_e64_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM result_queue_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM result_queue_d_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element mfpu_red_ready_q_reg was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/vmfpu.sv:2214]
WARNING: [Synth 8-3848] Net scan_data_o in module/entity lane does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/lane/lane.sv:36]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter FPUSupport bound to: 3'b111 
	Parameter FPExtSupport bound to: 1'b1 
	Parameter FixPtSupport bound to: 1'b1 
	Parameter INPUT_WIDTH bound to: 32'b00000000000000000000000000000111 
	Parameter PopcountWidth bound to: 32'b00000000000000000000000000000100 
INFO: [Synth 8-155] case statement is not full and has no default [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara_dispatcher.sv:331]
INFO: [Synth 8-155] case statement is not full and has no default [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara_dispatcher.sv:1298]
INFO: [Synth 8-155] case statement is not full and has no default [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara_dispatcher.sv:2483]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara_dispatcher.sv:2597]
INFO: [Synth 8-226] default block is never used [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara_dispatcher.sv:2796]
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter NrPEs bound to: 32'b00000000000000000000000000000110 
	Parameter InsnQueueDepth bound to: 224'b00000000000000000000000000000100000000000000000000000000000001000000000000000000000000000000001000000000000000000000000000000001000000000000000000000000000001000000000000000000000000000000010000000000000000000000000000000001 
	Parameter WIDTH bound to: 32'b00000000000000000000000000000011 
	Parameter STICKY_OVERFLOW bound to: 1'b0 
	Parameter WIDTH bound to: 32'b00000000000000000000000000000011 
	Parameter STICKY_OVERFLOW bound to: 1'b0 
WARNING: [Synth 8-5858] RAM read_list_d_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM write_list_d_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM read_list_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5858] RAM write_list_q_reg from Abstract Data Type (record/struct) for this pattern/configuration is not supported. This will most likely be implemented in registers
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter VInsnQueueDepth bound to: 2 - type: integer 
	Parameter ResultQueueDepth bound to: 32'b00000000000000000000000000000010 
	Parameter NrLanes bound to: 2 - type: integer 
	Parameter INPUT_WIDTH bound to: 32'b00000000000000000000000000000100 
	Parameter PopcountWidth bound to: 32'b00000000000000000000000000000011 
	Parameter WIDTH bound to: 32'b00000000000000000000000000000100 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000010 
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
WARNING: [Synth 8-5856] 3D RAM result_queue_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5856] 3D RAM result_queue_d_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[eew_vmask] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[scale_vl] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[conversion_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[eew_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vs2] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vs2] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[conversion_vs2] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[eew_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[swap_vs2_vd_op] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[use_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[emul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[fp_rm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[wide_fp_imm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[cvt_resize] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vstart] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vill] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vma] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vta] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[vtype][vlmul] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[hazard_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[hazard_vs2] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[hazard_vm] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_issue_q_reg[hazard_vd] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:88]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][eew_vmask] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][scale_vl] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][use_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][conversion_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][eew_vs1] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
WARNING: [Synth 8-6014] Unused sequential element vinsn_queue_q_reg[vinsn][1][vs2] was removed.  [/home/aitesam/Documents/GitHub/ara-build-playground/src/sldu/sldu.sv:85]
INFO: [Common 17-14] Message 'Synth 8-6014' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
	Parameter NrLanes bound to: 32'b00000000000000000000000000000010 
	Parameter DataWidth bound to: 32'b00000000000000000000000001000000 
	Parameter StrbWidth bound to: 32'b00000000000000000000000000001000 
	Parameter VInsnQueueDepth bound to: 1 - type: integer 
	Parameter MaskQueueDepth bound to: 32'b00000000000000000000000000000010 
	Parameter ResultQueueDepth bound to: 32'b00000000000000000000000000000010 
	Parameter INPUT_WIDTH bound to: 32'b00000000000000000000000010000000 
	Parameter PopcountWidth bound to: 32'b00000000000000000000000000001000 
	Parameter WIDTH bound to: 32'b00000000000000000000000010000000 
	Parameter MODE bound to: 1'b0 
	Parameter CNT_WIDTH bound to: 32'b00000000000000000000000000000111 
WARNING: [Synth 8-5856] 3D RAM mask_queue_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5856] 3D RAM result_queue_q_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5856] 3D RAM mask_queue_d_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-5856] 3D RAM result_queue_d_reg  for this pattern/configuration is not supported. This will most likely be implemented in registers
WARNING: [Synth 8-3936] Found unconnected internal register 'trimmed_stride_reg' and it is trimmed from '64' to '8' bits. [/home/aitesam/Documents/GitHub/ara-build-playground/src/masku/masku.sv:672]
WARNING: [Synth 8-3848] Net scan_data_o in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:39]
WARNING: [Synth 8-3848] Net axi_req_o in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:44]
WARNING: [Synth 8-3848] Net load_complete in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:78]
WARNING: [Synth 8-3848] Net store_complete in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:79]
WARNING: [Synth 8-3848] Net store_pending in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:80]
WARNING: [Synth 8-3848] Net pe_resp[3][vinsn_done] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:123]
WARNING: [Synth 8-3848] Net pe_resp[2][vinsn_done] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:123]
WARNING: [Synth 8-3848] Net addrgen_ack in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:125]
WARNING: [Synth 8-3848] Net addrgen_exception[cause] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception[tval] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception[tval2] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception[tinst] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception[gva] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception[valid] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:126]
WARNING: [Synth 8-3848] Net addrgen_exception_vstart in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:127]
WARNING: [Synth 8-3848] Net stu_operand_ready in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:193]
WARNING: [Synth 8-3848] Net addrgen_operand_ready in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:200]
WARNING: [Synth 8-3848] Net ldu_result_req in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:205]
WARNING: [Synth 8-3848] Net ldu_result_id[1] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:206]
WARNING: [Synth 8-3848] Net ldu_result_addr[1] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:207]
WARNING: [Synth 8-3848] Net ldu_result_wdata[1] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:208]
WARNING: [Synth 8-3848] Net ldu_result_be[1] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:209]
WARNING: [Synth 8-3848] Net ldu_result_id[0] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:206]
WARNING: [Synth 8-3848] Net ldu_result_addr[0] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:207]
WARNING: [Synth 8-3848] Net ldu_result_wdata[0] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:208]
WARNING: [Synth 8-3848] Net ldu_result_be[0] in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:209]
WARNING: [Synth 8-3848] Net vldu_mask_ready in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:307]
WARNING: [Synth 8-3848] Net vstu_mask_ready in module/entity ara does not have driver. [/home/aitesam/Documents/GitHub/ara-build-playground/src/ara.sv:308]
WARNING: [Synth 8-3331] design simd_mul__parameterized2 has unconnected port clk_i
WARNING: [Synth 8-3331] design simd_mul__parameterized2 has unconnected port rst_ni
WARNING: [Synth 8-3331] design stream_register__parameterized0 has unconnected port testmode_i
WARNING: [Synth 8-3331] design rr_arb_tree__parameterized2 has unconnected port rr_i[2]
WARNING: [Synth 8-3331] design rr_arb_tree__parameterized2 has unconnected port rr_i[1]
WARNING: [Synth 8-3331] design rr_arb_tree__parameterized2 has unconnected port rr_i[0]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[31]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[30]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[29]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[28]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[27]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[26]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[25]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[24]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[23]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[22]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[21]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[20]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[19]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[18]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[17]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[16]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[15]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[14]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[13]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[12]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[11]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[10]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[9]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[8]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[7]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[6]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[5]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[4]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[3]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[2]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[1]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port hart_id_i[0]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][63]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][62]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][61]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][60]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][59]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][58]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][57]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][56]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][55]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][54]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][53]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][52]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][51]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][50]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][49]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][48]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][47]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][46]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][45]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][44]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][43]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][42]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][41]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][40]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][39]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][38]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][37]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][36]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][35]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][34]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][33]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][32]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][31]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][30]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][29]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][28]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][27]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][26]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][25]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][24]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][23]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][22]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][21]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][20]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][19]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][18]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][17]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][16]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][15]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][14]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][13]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][12]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][11]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][10]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][9]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][8]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][7]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][6]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][5]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][4]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][3]
WARNING: [Synth 8-3331] design fpnew_opgroup_block__parameterized3 has unconnected port operands_i[2][2]
INFO: [Common 17-14] Message 'Synth 8-3331' appears 100 times and further instances of the messages will be disabled. Use the Tcl command set_msg_config to change the current settings.
---------------------------------------------------------------------------------
Finished RTL Elaboration : Time (s): cpu = 00:00:21 ; elapsed = 00:00:24 . Memory (MB): peak = 8639.922 ; gain = 91.695 ; free physical = 410 ; free virtual = 7586
---------------------------------------------------------------------------------

Report Check Netlist: 
+------+------------------+-------+---------+-------+------------------+
|      |Item              |Errors |Warnings |Status |Description       |
+------+------------------+-------+---------+-------+------------------+
|1     |multi_driven_nets |      0|        0|Passed |Multi driven nets |
+------+------------------+-------+---------+-------+------------------+
---------------------------------------------------------------------------------
Start Handling Custom Attributes
---------------------------------------------------------------------------------
---------------------------------------------------------------------------------
Finished Handling Custom Attributes : Time (s): cpu = 00:00:25 ; elapsed = 00:00:29 . Memory (MB): peak = 8662.734 ; gain = 114.508 ; free physical = 521 ; free virtual = 7697
---------------------------------------------------------------------------------
---------------------------------------------------------------------------------
Finished RTL Optimization Phase 1 : Time (s): cpu = 00:00:25 ; elapsed = 00:00:29 . Memory (MB): peak = 8662.734 ; gain = 114.508 ; free physical = 521 ; free virtual = 7697
---------------------------------------------------------------------------------
INFO: [Project 1-570] Preparing netlist for logic optimization
INFO: [Opt 31-141] Inserted 68 OBUFs to IO ports without IO buffers.

Processing XDC Constraints
Initializing timing engine
Completed Processing XDC Constraints

INFO: [Opt 31-140] Inserted 3 IBUFs to IO ports without IO buffers.
INFO: [Opt 31-138] Pushed 0 inverter(s) to 0 load pin(s).
Netlist sorting complete. Time (s): cpu = 00:00:00.01 ; elapsed = 00:00:00.01 . Memory (MB): peak = 9237.945 ; gain = 0.000 ; free physical = 418 ; free virtual = 7311
INFO: [Project 1-111] Unisim Transformation Summary:
  A total of 3 instances were transformed.
  IBUF => IBUF (IBUFCTRL, INBUF): 3 instances

RTL Elaboration Complete:  : Time (s): cpu = 00:01:19 ; elapsed = 00:00:57 . Memory (MB): peak = 9250.570 ; gain = 702.344 ; free physical = 230 ; free virtual = 6986
377 Infos, 325 Warnings, 0 Critical Warnings and 0 Errors encountered.
synth_design completed successfully
synth_design: Time (s): cpu = 00:01:19 ; elapsed = 00:00:57 . Memory (MB): peak = 9250.570 ; gain = 702.344 ; free physical = 230 ; free virtual = 6986

```