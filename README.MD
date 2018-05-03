# Site Information Tool

This project built with Python to get information about web sites.

**Status**: Development

# Endpoints

All endpoints will return json format.

**/dns**

Parameters: ['domain']

It will show dns records. You can extend record types like below:

```python
m_dns.types.append('AAAA')
```

**/port**

Parameters: ['domain', 'port']

It will show port status of domain you declared

**/find_admin**

Parameters: ['domain']

It will try to find admin panel of website. You can extend panel endpoints like below:

```python
m_admin_finder.endpoints.append('myadmin')
```

**/site_info**

Parameters: ['domain']

It will show site info for example:

- status_code
- title
- scripts
- css_list

# To-Do

- [ ] Improvement for admin finder
- [ ] Improvement for site info
- [ ] Front-end for the front-end
- [ ] Technology checker (Eg: wordpress, ghost, joomla)
- [ ] New ideas