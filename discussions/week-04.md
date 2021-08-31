# WEEk 04 - L.I.D. (Chapters 9, 10, and, 11)

## Liskov Substitution Principle

- LSP is primarily about guiding the use of inheritance. 
- Every "subtype" should be able to be used as its parent type "all the way up the chain"
- In the first image this is done well

![example of LSP as intended](https://user-images.githubusercontent.com/355561/131423517-9435406a-c5d8-4de5-b670-102f23be7ba0.png)

- in the second this is not

![example of the violation of LSP](https://user-images.githubusercontent.com/355561/131423705-69f4b145-498b-4b8e-b8cb-601b12da4399.png)

- the example in the book is long and convoluted 
- suffice it to say a simple violation of subsitutibility can cause a system's architecture to baloon out of control.

## Interface Segregation Principle

Picture of the BAD way:
![Picture of the BAD way](https://user-images.githubusercontent.com/355561/131425144-66adf14f-d892-4c42-a6d7-ffe7e5547698.png)

Better: add more interfaces!!

![Better: add more interfaces!!](https://user-images.githubusercontent.com/355561/131425439-309eed4e-5fa0-49b2-b44f-b53ac58f13ee.png)

- In general it is considered harmful to depend on code taht you don't actually use.
- In development time it can cause unnecessary recompilations and redeployments. 
  - Great example: [windows nano server](https://www.techradar.com/news/software/operating-systems/why-nano-server-is-the-most-vital-change-to-windows-server-since-windows-nt-3-5-1295803)
  - example of "old server" system [just for the image](https://redmondmag.com/articles/2015/02/05/next-windows-server-cloud.aspx)
  - content of this example to be discussed live in the show. Stay tuned for incoming youtube link after tomorrow night.... or in theory it is already there and I never removed this line of text. That souds like me.
- Something that carries baggage that you don't need can cause you troubles that you didn't expect.

## Dependency Inversion Principle
