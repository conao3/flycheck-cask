flycheck-cask
=============

Make Flycheck use Cask packages in Cask projects.


Installation
------------

As usual, from [MELPA](http://melpa.milkbox.net) and
[Marmalade](http://marmalade-repo.org/).

In your [`Cask`](https://github.com/rejeep/cask.el) file:

```lisp
(source melpa)

(depends-on "flycheck-cask")
```

In your `init.el`:

```lisp
(eval-after-load 'flycheck
  '(add-hook 'flycheck-mode-hook #'flycheck-cask-setup))
```

Usage
-----

Just use Flycheck as usual in Cask projects.

License
-------

This program is free software: you can redistribute it and/or modify it under
the terms of the GNU General Public License as published by the Free Software
Foundation, either version 3 of the License, or (at your option) any later
version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY
WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
PARTICULAR PURPOSE.  See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
this program.  If not, see http://www.gnu.org/licenses/.

See [COPYING](https://github.com/flycheck/flycheck-cask/blob/master/COPYING) for
details.
