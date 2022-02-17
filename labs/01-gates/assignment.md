# Lab 1: Cristóvão Matias Pedro Cristóvão

### De Morgan's laws

1. Equations of all three versions of logic function f(c,b,a):
https://latex.codecogs.com/svg.image?%5Cbg_white%20%5Cbegin%7Balign*%7D%20%20%20%20f(c,b,a)_%7B%5Ctextup%7BORG%7D%7D%20=&~%20%5Coverline%7Bb%7D%5C,a%20&plus;%20%5Coverline%7Bc%7D%5C,%5Coverline%7Bb%7D%5C%5C%20%20%20%20f(c,b,a)_%7B%5Ctextup%7BNAND%7D%7D%20=&~%20(%5Coverline%7Bb%7D%5C%20&plus;%20a%5C)%5C,%5Coverline%7Bc%7D%5C%20%5Coverline%7Bb%7D%5C%5C%20%20%20f(c,b,a)_%7B%5Ctextup%7BNOR%7D%7D%20=&~%20%5Coverline%7Bb%7D%5C,%20a%20%5Coverline%7Bc%7D%5C,%20b%5Cend%7Balign*%7D
```vhdl
architecture dataflow of demorgan is
begin
    f_org_o  <= (not(b_i) and a_i) or (not(c_i) and not(b_i));
    f_nand_o <= (not(b_i) nand a_i) or (not(c_i) nand not(b_i));
    f_nor_o  <= (not(b_i) and a_i) nor (not(c_i) and not(b_i));
end architecture dataflow;
```

3. Complete table with logic functions' values:

| **c** | **b** |**a** | **f(c,b,a)_ORG** | **f(c,b,a)_NAND** | **f(c,b,a)_NOR** |
| :-: | :-: | :-: | :-: | :-: | :-: |
| 0 | 0 | 0 | 1 | 1 | 0 |
| 0 | 0 | 1 | 1 | 0 | 0 |
| 0 | 1 | 0 | 0 | 1 | 1 |
| 0 | 1 | 1 | 0 | 1 | 1 |
| 1 | 0 | 0 | 0 | 1 | 1 |
| 1 | 0 | 1 | 1 | 1 | 0 |
| 1 | 1 | 0 | 0 | 1 | 1 |
| 1 | 1 | 1 | 0 | 1 | 1 |

### Distributive laws

1. Screenshot with simulated time waveforms. Always display all inputs and outputs (display the inputs at the top of the image, the outputs below them) at the appropriate time scale!

   ![your figure]()

2. Link to your public EDA Playground example:

   [https://www.edaplayground.com/...](https://www.edaplayground.com/...)
