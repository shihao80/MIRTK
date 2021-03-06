:orphan:

.. Auto-generated by help-rst from "mirtk evaluate-jacobian -h" output

evaluate-jacobian
=================

.. program:: evaluate-jacobian


Synopsis
--------

::

    evaluate-jacobian <target> <output> <dof> [options]
    evaluate-jacobian <target> <dof> [options]


Description
-----------

.. include:: _descriptions/evaluate-jacobian.rst



Arguments
---------

.. option:: target

   Target image.

.. option:: output

   Output Jacobian map.

.. option:: dof

   Input transformation.


Command options
---------------

.. option:: -total

   Total Jacobian. (default)

.. option:: -local

   Local Jacobian only.

.. option:: -global

   Global Jacobian only.

.. option:: -relative

   Local Jacobian divided by global Jacobian.

.. option:: -log

   Log of total Jacobian.

.. option:: -padding <value>

   Target padding value. (default: none)

.. option:: -outside <value>

   Outside determinant value. (default: 0)

.. option:: -Tt <value>

   Temporal origin of target image. (default: _torigin)

.. option:: -St <value>

   Temporal origin of source image. (default: _torigin + _dt)

.. option:: -ss [fast]

   Force use of scaling-and-squaring for SV FFD. (default: SV FFD integration method)

.. option:: -noss

   Do not use scaling-and-squaring for SV FFD.

.. option:: -disp [on|off]

   Evaluate Jacobian of linearly interpolated displacement field. (default: off)

.. option:: -velo [on|off]

   Evaluate Jacobian of velocity field parameterization for SV/TD FFD. (default: off)

.. option:: -float

   Output values as single-precision floating point.

.. option:: -double

   Output values as double-precision floating point.

.. option:: -real

   Output values as floating point with default precision.

.. option:: -threshold <value>

   Lower Jacobian determinant threshold used when computing -log. (default: 1e-4)


Standard options
----------------

.. option:: -v, -verbose [n]

   Increase/Set verbosity of output messages. (default: 0)

.. option:: -debug [level]

   Increase/Set debug level for output of intermediate results. (default: 0)

.. option:: -version [major.minor]

   Print version and exit or set version to emulate.

.. option:: -revision

   Print revision (or version) number only and exit.

.. option:: -h, -help

   Print help and exit.


Terminal options
----------------

.. option:: -color, -nocolor

   Enable/disable colored output. (default: off)


Parallelization options
-----------------------

.. option:: -threads <n>

   Use maximal <n> threads for parallel execution. (default: automatic)
