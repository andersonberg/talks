Um dos frameworks mais populares para criar APIs RESTful em Python é o Django Rest Framework. Baseado no Django (como o próprio nome já diz), possui a mesma flexibilidade e rapidez no desenvolvimento. Vamos falar sobre como construir sua API do zero e consumir utilizando o arduino.

# Django Rest Framework

A página do DRF lista algumas vantagens de usar o framework:

 - API navegável: Vem com uma interface web integrada
 - Mecanismos de autenticação inclusos
 - Serialização tanto com ORM quanto sem
 - Totalmente customizável
 - Extensa documentação [http://www.django-rest-framework.org/](http://www.django-rest-framework.org/)
 - Usado por grandes companhias como Mozilla, Heroku e Eventbrite

<!-- O objetivo deste post é mostrar um guia, quase como um quickstart para configurar e rodar sua API e conseguir consumí-la externamente com o arduino.

    pip install djangorestframework
    pip install markdown -->

O processo de instalação e criação de um novo projeto com o DRF são semelhantes ao Django. É tudo muito simples e rápido e pode ser visto no "quickstart" no próprio site do DRF. Nosso objetivo aqui é mostrar como funciona o DRF e alguns detalhes de implementação.


## Models
O primeiro passo é definir os models, assim como fazemos no django. Por exemplo, nossa classe Professor:

    class Professor(models.Model):
        nome = models.TextField()
        cpf = models.IntegerField()
        tag = models.TextField()

        class Meta:
            ordering = ('nome',)
