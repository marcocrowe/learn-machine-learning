
# Data Types

In the context of machine learning, different types of data require different types of processing. The most common data types are:

- Categorical
  - Nominal
  - Ordinal
- Numerical
  - Interval
  - Ratio

Numerical data can be further divided into interval and ratio data. Interval data has no true 
zero i.e temperature, where 0 degrees Celsius is not the absence of temperature, you have a temperature of 0 degrees Celsius. On the other hand, ratio data has a true zero i.e weight, where 0 kg means no weight.

```mermaid
graph TB;
%% If you see this code instead of an image, please add this extension to your browser, such as:
%% https://chrome.google.com/webstore/detail/markdown-diagrams/pmoglnmodacnbbofbgcagndelmgaclel
  dataTypes(Data Types)
  dataTypes-->categorical(Categorical)
  dataTypes-->numerical(Numerical)
  categorical-->nominal(Nominal)
  categorical-->ordinal(Ordinal)
  numerical-->interval(Interval)
  numerical-->ratio(Ratio)
  nominal-->nominalExample((Gender, <br/>Language))
  ordinal-->ordinalExample(("Happiness, <br/> {sad, okay,<br/> happy}"))
  interval-->intervalExample((Celsius <br/>or Fahrenheit <br/>temperature <br/>scale))
  ratio-->ratioExample((Height, <br/>Weight))
  nominalExample-->nominalOrder(NOT Ordered)
  ordinalExample-->ordinalOrder(Ordered)
  intervalExample-->intervalOrder(Ordered)
  ratioExample-->ratioOrder(Ordered)
```
