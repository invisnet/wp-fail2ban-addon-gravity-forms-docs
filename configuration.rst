.. _configuration:

Configuration
=============

Typical Settings
""""""""""""""""

#. Copy `wordpress-gravityforms-extra.conf` to your `fail2ban/filters.d` directory
#. Edit `jail.local` to include something like:

.. code-block:: sh

   [wordpress-gravityforms-extra]
   enabled = true
   filter = wordpress-gravityforms-extra
   logpath = /var/log/auth.log
   maxretry = 1
   port = http,https

3. Reload or restart `fail2ban`


