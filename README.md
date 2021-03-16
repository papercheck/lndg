# lndg
Lite GUI web interface to analyze lnd data.

## Setup
1. Run bitcoind
2. Run lnd
3. Build required py file for your system to interact with lnd grpc: https://github.com/lightningnetwork/lnd/blob/master/docs/grpc/python.md#setup-and-installation
4. Clone respository
5. Place the 2 ouput files from step 3 inside the repository at: lndg/gui/
6. A settings file is required at lndg/settings.py (default django setting file + 'gui' added to your installed apps inside the file)
7. Make migrations and migrate all database objects (python manage.py makemigrations && python manage.py migrate)
8. Run the server via apache or development server (python manage.py runserver IP:PORT)
