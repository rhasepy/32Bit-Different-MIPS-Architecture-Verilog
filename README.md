# 32Bit-Different-MIPS-Architecture-Verilog


<h2>Supported Instructions</h2>

<table style="width:100%">
  <tr>
    <th>Instructions</th>
    <th>RTL Representations</th>
   </tr>
  
  <tr>
    <th>lw</th>
    <th>R[t] = Mem [R[s]] + signImm16]</th>
   </tr>
  
   <tr>
    <th>sw</th>
    <th>Mem [R[s]] + signImm16] = R[t]</th>
   </tr>
  
   <tr>
    <th>j</th>
    <th>PC = JumpAddress</th>
   </tr>

   <tr>
    <th>jal</th>
    <th>PC = JumpAddress and R[11111] = PC + 8</th>
   </tr>
  
   <tr>
    <th>jr</th>
    <th>PC = R[11111] or PC = R[s]</th>
   </tr>
  
   <tr>
    <th>beq</th>
    <th>if (R[s] == R[t]) PC = PC + 4 + BranchAddress</th>
   </tr>
  
   <tr>
    <th>bne</th>
    <th>if (! (R[s] == R[t]) ) PC = PC + 4 + BranchAddress</th>
   </tr>
  
   <tr>
    <th>addn</th>
    <th>
         R[s] = R[s] + R[t]
         if(R[s] + R[t] == 0) R[d] = 1
         else if(R[s] + R[t] == 1) R[d] = 2
         else R[d] = 3
    </th>
   </tr>
  
   <tr>
    <th>subn</th>
      <th> 
         R[s] = R[s] - R[t]
         if(R[s] - R[t] == 0) R[d] = 1
         else if(R[s] - R[t] == 1) R[d] = 2
         else R[d] = 3
      </th>
   </tr>
  
   <tr>
    <th>xorn</th>
      <th>         
         R[s] = R[s] xor R[t]
         if(R[s] xor R[t] == 0) R[d] = 1
         else if(R[s] xor R[t] == 1) R[d] = 2
         else R[d] = 3
      </th>
    </tr>
    
   <tr>
    <th>andn</th>
      <th>         
         R[s] = R[s] and R[t]
         if(R[s] and R[t] == 0) R[d] = 1
         else if(R[s] and R[t] == 1) R[d] = 2
         else R[d] = 3
      </th>
    </tr>
  
   <tr>
    <th>orn</th>
      <th>         
         R[s] = R[s] or R[t]
         if(R[s] or R[t] == 0) R[d] = 1
         else if(R[s] or R[t] == 1) R[d] = 2
         else R[d] = 3
      </th>
  </tr>
  
   <tr>
    <th>ori</th>
    <th>R[t] = R[s] or zeroExtendImm</th>
  </tr>
  
   <tr>
    <th>lui</th>
    <th>R[t] = {imm16, 16'b0}</th>
  </tr>
</table>
