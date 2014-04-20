#composer.lock file

* It contains all the installed dependencies and their versions (commit number).

* The first time you do a `composer install` composer creates the lock file.

* If the lock file is already present `composer install` will install the exact versions from there.

---

#Pro tips

* Always commit your composer.json and composer.lock file (all the team will work on the exact same versions)

* On production, always install dependencies from `composer.lock`
