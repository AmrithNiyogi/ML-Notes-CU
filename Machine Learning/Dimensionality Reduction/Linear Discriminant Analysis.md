- Supervised method
- Find a low-dim space such that when x is projected over w, samples of all classes are well separated.
- Let,  $X = \{x^{t},r^{t}\} \ such \ that \ r^{t}= 1 \ if \ x^{t} \epsilon C_{1 } \ and \ r^{t}=0 \ if \ x^{t} \epsilon C_2$
	- $\mu_{1} \ and \ m_{1}$ are the means of samples from $C_{1}$ before and after projections
	- $$m_{1} = \frac{\sum_{t}w^{T}x^{t}r^{t}}{\sum_{t}r^t} = w^{T}\mu_{1}$$
	- $\mu_{2} \ and \ m_{2}$ are the means of samples from $C_{1}$ before and after projections
	- $$m_{2}= \frac{\sum_{t}w^{T}x^{t}(1-r^{t})}{\sum_{t}(1-r^t)} = w^{T}\mu_{2}$$
- Scattering of samples from $C_{1} \ and \ C_{2}$ after projection:
	- $$s^{2}_{1} = \sum_{t}(w^{T}x^{t}-m_{1})^{2}r^{t}$$
	- $$s^{2}_{2} = \sum_{t}(w^{T}x^{t}-m_{2})^{2}(1-r^{t})$$
- After projection of samples for two classes
	- Their mean should be as far as possible, that is $|m_{1} - m_{2}|$ should be large
	- Scattering between examples of classes should be in as small a region as possible, that is $s_{1}^2 + s_{2}^2$ should be small