# Full-adder-implementation-using-if-else-condtional-statements
`timescale 1ns / 1ps


module FA_if(
    input a,
    input b,
    input c,
    output reg sum,
    output reg cout
    );
    always@(*)
    begin
    if (a==0 & b==0 & c==0)
        begin
        sum=0; cout=0;
        end
       
        else if (a==0 & b==0 & c==1)
        begin
         sum=1;  cout=0;
        end
       
        else if (a==0 & b==1 & c==0)
        begin
         sum=1;cout=0;
         end
       
        else if (a==0 & b==1 & c==1)
        begin
        sum=0; cout=1;
        end
        
        else if(a==1 & b==0 & c==0)
        begin
        sum=1; cout=0;
        end
        
        else if (a==1 & b==0 & c==1)
        begin
        sum=0; cout=1;
        end
        
        else if (a==1 & b==1 & c==0)
        begin
        sum=0; cout=1;
        end
       
        else if(a==1 & b==1 & c==1)
        begin
        sum=1; cout=1;
        end
    end
endmodule
