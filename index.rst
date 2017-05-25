.. title: home
.. hidetitle: True
.. slug: index
.. date: 2017-05-17 11:30:44 UTC+03:00
.. tags:
.. category:
.. link:
.. description:
.. type: text

ВАШ сайт

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
