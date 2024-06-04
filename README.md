# Trabalho 1 - Projeto de Fonte de Tensão Ajustável 3V-12v
Projeto realizado no primeiro semestre do curso de Bacharelado em Ciências de Computação, para a disciplina '[SSC0180] – Eletrônica para Computação', ministrada pelo professor Eduardo do Valle Simões, da USP de São Carlos.


# Integrantes - Grupo 17

| **Nome**              | **N°USP**|
|--------------------------------|----------|
| Bruna Izabel da Silva Pereira| 15635441 | 
| Camilli Gabrielli Ramos Muniz| 15635722 |
| [Laura Fernandes Camargos](https://github.com/laurafcamargos)| 13692334 |
| Sandy da Costa Dutra| 12544570 |



# Objetivo
Projetar uma fonte de tensão retificadora, ajustável entre 3V e 12V, com capacidade de 100mA.


# Diagrama da Fonte
![Diagrama da fonte no software Falstad](imagens/falstad_circuito.jpg "Diagrama da fonte no software Falstad")

[Link para o circuito no Falstad]([https://tinyurl.com/yengesgj](https://www.falstad.com/circuit/circuitjs.html?ctz=CQAgjCAMB0l3BWc0DMAOSAWBB2TY0A2SQnSATkJExxCUxToFMBaMMAKADcRDNxivfigBMUcL0jgc5aMQQQpS6Ag4AVISFECpYQVP4ww+HKJFoo0EShyEUetI7THykWixQqEhAvZG4EEWxsVjBaGHJIjgB3cEx+Sjj+fypIGJ0tMSCpbTTYvV1BbIy8pJBEsKpEtIATaSqqYu0xGqYAMwBDAFcAGwAXDjrK8sbMQqkW9u7+wZAmsRQsEbmQVs7egbrigq0lxMn1mYBzMpTTnDElDgAnakTEzArbcUIMDhR+ADkAeQBlX++LAAWgBRT4ggBKEjA0BwxhQgWc5HMYHgIlY4TmsHgONxkDQ-DAjE4AC87o1vOT6isfv9AaDwRD0o8GnR4stSizqYjqWk+rwLnNKRcJpTdCA2DAEGhyN4EAgPt44fLLHCaIRyGNfP49BBUXBVlMNukRXMxiBTcNSrhWQh2dVmftKVyUChUiaRBNBTgCXNBdbzNzkbzHVRXVQXa8oKGtFHiBY3RY0rd47GLKnFoYtK5Shmoz7hFHkyAZY1BaW0+IwJ6OGF+KnPen8btCeAcZZIEEMHi8YwIUwAM4ASwHfQ6ADsAMZMdIIYPDVNW9KL54N5u5oJCqikLJij26Z6mh2xI9UG0c2uEMQMMQPbTDA7TPosHpMIbiZSQTi3G-U39nXR4HSYxkkpBFd3dWJwK3ahmj3WJ-2dJ1IK0QJll-Y9YNvCN7hQ6DEkzC9PXIVDsNImDP0QRpPARSgRAIVxHhoJNsT1DgAAdynZERBU1QsLEUaMbCkAs-TECseLEQTSlExMSwIot0grOS+MrUoJN47j-Q4AB7IUJAMCgSM9SxLhWfwtA4IA)

# Escolha de Componentes

| Quantidade  | Componente  | Especificações   | Valor  |
|---|---|---|---|
| 1 | [Ponte de Diodos](https://www.baudaeletronica.com.br/ponte-retificadora-kbpc1010.html) | Ponte Retificadora KBPC1010 |R$3,67| 
| 1 | [Capacitor](https://produto.mercadolivre.com.br/MLB-1673538375-capacitor-d97-eletrolitico-smd-560uf-25v-emb-10-pcs-_JM?matt_tool=87716990&matt_word=&matt_source=google&matt_campaign_id=12413740998&matt_ad_group_id=119070072438&matt_match_type=&matt_network=g&matt_device=c&matt_creative=500702333978&matt_keyword=&matt_ad_position=&matt_ad_type=pla&matt_merchant_id=109554163&matt_product_id=MLB1673538375&matt_product_partition_id=337120033364&matt_target_id=pla-337120033364&gclid=CjwKCAjwuvmHBhAxEiwAWAYj-Ay7yDPELDOSm39X_i7gBUjtOCS0CwJmOsPk51wYcrQWBM-lYwfB2xoCgIcQAvD_BwE) |560µF, 25V|R$1,10|
| 1 | [LED](https://www.baudaeletronica.com.br/led-de-alto-brilho-10mm-vermelho.html) |Vermelho 3V - 3,3V 30mA|R$0,70|
| 1 | [Diodo Zener](https://www.baudaeletronica.com.br/diodo-zener-1n4743-13v-1w.html) |1N4743 [13V / 1W]|R$0,19|
| 1 | [Potenciômetro](https://www.baudaeletronica.com.br/potenciometro-linear-de-10k-10000.html) |10000Ω|R$1,61|
| 1 | [Resistor 820](https://www.baudaeletronica.com.br/resistor-680r-5-2w.html) |680Ω +/-5%, 2W|R$0,38|
| 1 | [Resistor 1k](https://www.baudaeletronica.com.br/resistor-1k-5-1w.html) |1000Ω +/-5%, 1W|R$0,18|
| 1 | [Resistor 100](https://www.baudaeletronica.com.br/resistor-3k9-5-2w.html) |3900Ω +/-5%, 2W|R$0,38|
| Total | | |R$36,20|


# Projeto Esquemático do PCB no Software Eagle
![Esquema do Eagle](imagens/eagle_circuito.jpg "Esquema do Eagle")

![Esquema do Eagle](imagens/esquema_front.jpg "Esquema do Eagle")

![Esquema do Eagle](imagens/esquema_back.jpg "Esquema do Eagle")

![Esquema do Eagle](imagens/esquema_board.jpg "Esquema do Eagle")

![Esquema do Eagle](imagens/esquema_3d.jpg "Esquema do Eagle")


# Vídeos Explicativos
[Vídeo explicando cálculos]()


[Vídeo explicando as etapas]()
