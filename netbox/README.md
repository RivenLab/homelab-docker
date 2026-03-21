.env example for this stack:

text
app_domain=netbox.example.com
app_data_path=/mnt/gfs/netbox

# netbox.env, postgres.env, redis.env etc. stay like upstream,
# just make sure DB/Redis passwords match across those files.


Create directories on GlusterFS once:

```bash
mkdir -p /mnt/gfs/netbox/{media,reports,scripts,postgres,redis,redis-cache}
```
