# hello-world
Just begin test
//Well, I am not so sure which type of program for this editor.
//So I just set most simple MATLAB print here

fprintf('\nHello world.');
fprintf('\nI prefer Fry Chicken more than Apple Pie!');

//After pull and merge, let's do something different.

module Fulladder (
      input A,
      input B,
      input Ci,
      output S,
      output Co
      )
  
  halfadder HA1(A,B,ps,pc);
  halfadder HA2(ps,Ci,S,fc);
  OR(Co,fc,pc);
endmodule

module halfadder(
      input ha,
      input hb,
      output hs,
      output hc
      )

  AND(hc,ha,hb);
  XOR(hs,ha,hb);
endmodule


