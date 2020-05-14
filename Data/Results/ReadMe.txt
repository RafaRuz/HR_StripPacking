This file include packing results of all the instances used for the paper "A Block-based Layer Building Approach for the 2D Guillotine Strip Packing Problems",
The folder OG is the results for the 2DSP-OG;
The folder RG is the results for the 2DSP-RG;
Each folder include a summary file and a solution folder include the packing result for each instance.
--------------------------------------------------------------------------------------------------------------------------------------------
The naming conventions for results file:
T7e.txt.pack:
 T7e.txt:             Instances name
--------------------------------------------------------------------------------------------------------------------------------------------
File-structure: each results file is described as follows:

(Data for the result)
Line 01:      h: H                                   :The found height
                         				 h::label
                                                           H:The found minimum height of the strip
Line 02:      time:t                                :Time to find final best solution
                         			      time: label
                                                            t:Time to find final best solution(s)

(Data for the strip)
Line 03:      W LB                               :size of the strip
                                                         W:strip width
                                                        LB:strip heigth(lower bound)
Line 04:      n                                       :number of items
Line 04+1:      w h                               : data for item 1
                                                          w: width of item 1
                                                    	h : height of item 1
.....................
Line 04+i                                            :data for item  i
.....................
Line 04+n                                           :data for item  n

(Data for packed item)
Line 05+n:    m                                  	     :number of packed item
Line 05+n+1:  w h  x1 y1 x2 y2 seq              :data for packed item 1
							   w:width of the item
							    h:height of the item
						       x1,y1:the coordinate of the corner that is closet to origin of packed item 1
                                                    	       x2,y2:the coordinate of the corner that is furthest to origin of packed item 1
                                                    	           seq:the packed oreder of packed item 1
...................................................
Line 05+n+i                                                    :data for packed item i
...................................................
Line 05+n+m                                                  :data for packed item m

                 
---------------------------------------------------------------------------------------------------------------------------------------------