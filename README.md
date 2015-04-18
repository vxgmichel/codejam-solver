codejam-solver
==============

A solver module to abstract the recurrent parts of problem solving.

Requirement
-----------

 - Python 2.7
 - Pytest (optional)

Features
--------

 - File operations
 - Multiprocessing
 - Command line interface

Example
-------
  
    from solver import solver

    @solver
    def square(lines):
        """Return the square of the given argument."""
        return int(lines[0]) ** 2

    if __name__ == "__main__":
        square.from_cli()

Usage
-----

    $ python some_problem.py some_input_file.in
    $ python some_problem.py -h # For more information

Performance
-----------

Results in seconds for large input of the [Infinite House of Pancakes][ihp] 
problem. All the resources are in the `example` directory. 

| Multiprocessing | No   | Yes |
|-----------------|------|-----|
| CPython         | 10.5 | 2.9 |
| PyPy            | 1.2  | 0.4 |

[ihp]: https://code.google.com/codejam/contest/6224486/dashboard#s=p1

Contact
-------

Vincent Michel: vxgmichel@gmail.com