.. Permission is granted to copy, distribute and/or modify this
.. document under the terms of the GNU Free Documentation License,
.. Version 1.1 or any later version published by the Free Software
.. Foundation, with no Invariant Sections, no Front-Cover Texts
.. and no Back-Cover Texts. A copy of the license is included at
.. Documentation/media/uapi/fdl-appendix.rst.
..
.. TODO: replace it to GFDL-1.1-or-later WITH no-invariant-sections

.. _DMX_REMAP_PID:

===============
DMX_REMAP_PID
===============

Name
----

DMX_REMAP_PID


Synopsis
--------

.. c:function:: int ioctl(fd, DMX_REMAP_PID, __u16[2])
    :name: DMX_REMAP_PID


Arguments
---------

``fd``
    File descriptor returned by :c:func:`open() <dvb-dmx-open>`.

``__u16[2]``
    __u16[0] original pid, __u16[1] is new pid


Description
-----------

This ioctl call allow change the pid in ts stream.

Return Value
------------

On success 0 is returned, on error -1 and the ``errno`` variable is set
appropriately. The generic error codes are described at the
:ref:`Generic Error Codes <gen-errors>` chapter.
