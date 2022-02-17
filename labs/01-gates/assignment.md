# Lab 1: Cristóvão Matias Pedro Cristóvão

### De Morgan's laws

1. Equations of all three versions of logic function f(c,b,a):
<img src="https://latex.codecogs.com/gif.image?\dpi{110}&space;\bg_white&space;\begin{align*}&space;&space;&space;&space;f(c,b,a)_{\textup{ORG}}&space;=&~&space;\overline{b}\,a&space;&plus;&space;\overline{c}\,\overline{b}\\&space;&space;&space;&space;f(c,b,a)_{\textup{NAND}}&space;=&~&space;(\overline{b}\&space;&plus;&space;a\)\,\overline{c}\&space;\overline{b}\\&space;&space;&space;f(c,b,a)_{\textup{NOR}}&space;=&~&space;\overline{b}\,&space;a&space;\overline{c}\,&space;b\end{align*}" title="\bg_white \begin{align*} f(c,b,a)_{\textup{ORG}} =&~ \overline{b}\,a + \overline{c}\,\overline{b}\\ f(c,b,a)_{\textup{NAND}} =&~ (\overline{b}\ + a\)\,\overline{c}\ \overline{b}\\ f(c,b,a)_{\textup{NOR}} =&~ \overline{b}\, a \overline{c}\, b\end{align*}" />
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
