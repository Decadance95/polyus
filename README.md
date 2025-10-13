Traceback (most recent call last):
  File "/usr/local/lib/python3.7/site-packages/celery/app/trace.py", line 385, in trace_task
    R = retval = fun(*args, **kwargs)
  File "/usr/local/lib/python3.7/site-packages/celery/app/trace.py", line 650, in __protected_call__
    return self.run(*args, **kwargs)
  File "/home/hhive/dist/apps/ldap/tasks.py", line 222, in run
  File "/home/hhive/dist/apps/metrics/decorators.py", line 57, in wrapped
  File "/home/hhive/dist/apps/ldap/tasks.py", line 197, in sync_user
  File "/home/hhive/dist/apps/metrics/decorators.py", line 57, in wrapped
  File "/home/hhive/dist/apps/ldap/tasks.py", line 387, in sync_user_groups
  File "/home/hhive/dist/apps/metrics/decorators.py", line 57, in wrapped
  File "/home/hhive/dist/apps/ldap/connections.py", line 491, in get_groups_by_user_sid
  File "/home/hhive/dist/apps/ldap/connections.py", line 556, in _prepare_iterable
  File "/usr/local/lib/python3.7/site-packages/ldap3/extend/standard/PagedSearch.py", line 68, in paged_search_generator
    None if cookie is True else cookie)
  File "/usr/local/lib/python3.7/site-packages/ldap3/core/connection.py", line 786, in search
    check_names=self.check_names)
  File "/usr/local/lib/python3.7/site-packages/ldap3/operation/search.py", line 372, in search_operation
    request['filter'] = compile_filter(parse_filter(search_filter, schema, auto_escape, auto_encode, validator, check_names).elements[0])  # parse the searchFilter string and compile it starting from the root node
  File "/usr/local/lib/python3.7/site-packages/ldap3/operation/search.py", line 215, in parse_filter
    raise LDAPInvalidFilterError('malformed filter')
ldap3.core.exceptions.LDAPInvalidFilterError: malformed filter
