# OnlineShop
Website for shopping http://mebecun.com

## Environment
- Python 3.4.3
- Django 1.8.3
- Postgres 9.4

### Connect to Database
``
psql -h localhost -d onlineshop -U kunn -W
``

### Additional modules
- Pillow + Requests
```
pip install Pillow
pip install Requests
```

### Deployment Setup

Setup ~/.ssh/config
```
Host mebecun
  HostName ec2-52-76-35-183.ap-southeast-1.compute.amazonaws.com
  User ubuntu
  IdentityFile /Users/kunn/Desktop/mebecun.pem
```

repo

``
git add remote production ubuntu@peer-review:{bare repo}/
``

deploying

``
git push production master
``
