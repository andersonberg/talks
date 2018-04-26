Um dos frameworks mais populares para criar APIs RESTful em Python é o Django Rest Framework. Baseado no Django (como o próprio nome já diz), possui a mesma flexibilidade e rapidez no desenvolvimento. Vamos falar sobre como construir sua API do zero e consumir utilizando o arduino.

## Django Rest Framework

A página do DRF lista algumas vantagens de usar o framework:

 - API navegável: Vem com uma interface web integrada
 - Mecanismos de autenticação inclusos
 - Serialização tanto com ORM quanto sem
 - Totalmente customizável
 - Extensa documentação [http://www.django-rest-framework.org/](http://www.django-rest-framework.org/)
 - Usado por grandes companhias como Mozilla, Heroku e Eventbrite

O objetivo deste post é mostrar um guia, quase como um quickstart para configurar e rodar sua API e conseguir consumí-la externamente com o arduino.

    pip install djangorestframework
    pip install markdown
