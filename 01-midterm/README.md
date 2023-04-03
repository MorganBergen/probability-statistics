# midterm 2

###  contents

1.  [5.25](#525)
2.  [5.27](#527)
3.  [5.66](#566)
4.  [5.67](#567)
5.  [6.8](#68)
6.  [6.32](#632)
7.  [6.34](#632)
8.  [6.55](#655)
9.  [6.66](#666)
10. [6.17](#617)
11. [6.20](#620)
12. [8.27](#827)
13. [8.30](#830)

### 5.25

suppose that for a very large shipment of integrated-circuit chips, the probability of failure for any one chip 0.10.  assuming that the assumptions underlying the binomial distributions are met, find the probability that at most 3 chips fail in a random sample of 20.

###  























**example 5.3**  a large chain retailer purchases a certain kind of electronic device from a manufacturer.  the manufacturer indicates that defective rate of the device is 3%.

a.  the inspector of the retailer randomly picks 20 items from a shipment.  what is the probability that there will be at least one defective item among these 20?

denote by $X$ the number of defective devices among the 20; $b(x; 20, 0.03)$

$$P(X \geq 1) = 1 - P(X = 0) = 1 - b(0; 20, 0.03) = (1 - 0.03^{0})(0.97^{20 - 0}) = 0.4562$$

b.  suppose that the retailer receives 10 shipments in a month and the inspector randomly tests 20 devices per shipment.  what is the probability that there will be 3 shipments containing at least one defective device?

denote by $Y$ the number of shipments containing at least one defective item $b(y; 10, 0.4562)$

$$P(Y = 3) = {{10}\choose{3}} 0.4562^{3}(1 - 0.4562)^{10 - 3} = 0.1602$$


