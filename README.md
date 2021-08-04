# ansible-wireguardservers
Ansible playbook and role to create side-to-side or mulit-side wireguard setups

## Examples:
```
                +--------+                +--------+
+-------+       |        |                |        |       +-------+
| Local |       |   wg   |                |   wg   |       | Local |
|  Lan  +<----->+ server +                + server +<----->+  Lan  |
|   #1  |       |   #1   |                |   #2   |       |   #2  |
+-------+       |        |                |        |       +-------+
                +--------+                +--------+
                          \              /
                           \            /
                            +----------+
                            |          |
                            + Internet +
                            |          |
                            +----------+



                +--------+                +--------+
+-------+       |        |                |        |       +-------+
| Local |       |   wg   |                |   wg   |       | Local |
|  Lan  +<----->+ server +                + server +<----->+  Lan  |
|   #1  |       |   #1   |                |   #2   |       |   #2  |
+-------+       |        |                |        |       +-------+
                +--------+                +--------+
                          \              /
                           \            /
                            +----------+
                            |          |
                            + Internet +
                            |          |
                            +----------+
                           /
                          /                 
                +--------+                
+-------+       |        |
| Local |       |   wg   |
|  Lan  +<----->+ server +
|   #3  |       |   #3   |
+-------+       |        |
                +--------+                
               


                +--------+                +--------+
+-------+       |        |                |        |       +-------+
| Local |       |   wg   |                |   wg   |       | Local |
|  Lan  +<----->+ server +                + server +<----->+  Lan  |
|   #1  |       |   #1   |                |   #2   |       |   #2  |
+-------+       |        |                |        |       +-------+
                +--------+                +--------+
                          \              /
                           \            /
                            +----------+
                            |          |
                            + Internet +
                            |          |
                            +----------+
                           /            \
                          /              \                 
                +--------+                +--------+
+-------+       |        |                |        |       +-------+
| Local |       |   wg   |                |   wg   |       | Local |
|  Lan  +<----->+ server +                + server +<----->+  Lan  |
|   #3  |       |   #3   |                |   #4   |       |   #4  |
+-------+       |        |                |        |       +-------+
                +--------+                +--------+
```

## Project dependencies

### Python
* [netaddr](https://pypi.org/project/netaddr/)

```bash
pip install netaddr
```
