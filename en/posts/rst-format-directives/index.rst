.. title: rst-format directives.
.. slug: rst-format-directives
.. date: 2017-05-24 14:07:42 UTC+03:00
.. tags:
.. category:
.. link:
.. description:
.. type: text

Блоки кода для ``rst-format``
++++++++++++++++++++++++++++++

Директива кода была частью Docutils, начиная с версии 0.9, и поддерживаются два псевдонима, кодовый блок и исходный код.

Давайте добавим следующий фрагмент кода в демонстрационный пример и посмотрим, как он выглядит:

``.. code-block:: python``

   ``:number-lines:``

.. code-block:: python
 :number-lines:

 def sieve_of_eratosthenes():
       factors = defaultdict(set)
     for n in count(2):
         if factors[n]:
             for m in factors.pop(n):
                 factors[n+m].add(m)
         else:
             factors[n*n].add(n)
             yield n


or

``.. code-block:: css``

.. code:: css

  div.sidebar,.sidebar {
      position: fixed;
      top: 0;
      bottom: 0;
       [...]
