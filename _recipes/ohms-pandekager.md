---
title: Ohms Pandekager
---
*af Mads Ohm Larsen*

Antal brugere
-------------
1-3

Udviklingsmiljø
---------------
 * 1/8 kg mel
 * 1 æg
 * 1/8 øl
 * 1/4 l mælk
 * lidt sukker
 * lidt vanillesukker
 * lidt olie
 * lidt smør/margarine
 * pander

Program
-------

{% highlight java %}
import skab.ingredienser;

Skål storSkål = new Skål();

storSkål.add(mel);
storSkål.add(æg);
storSkål.mix();
storSkål.add(mælk+øl);
storSkål.mix();
storSkål.add(sukker+vanillesukker);
storSkål.mix();
storSkål.add(olie);
storSkål.mix();

Pande p = new Pande();

while(!storSkål.tom()) {
  p.add(storSkål.getDej());
  p.steg();
  p.vend();
  p.steg();
  this.eat(p.getPandekage());
}
{% endhighlight %}

Sidenote
--------
Lav ALTID 8-dobbelt eller 16-dobbelt portion
