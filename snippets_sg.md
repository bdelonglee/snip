#### SG Load MGL wrapper
```bash
>envi -c mgl_shotgun_api3
>python
Python 3.9.19 (main, May 20 2024, 05:19:58) 
[GCC 8.5.0 20210514 (Red Hat 8.5.0-22)] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> import mgl_shotgun
>>> sg_obj=mgl_shotgun.MglShotgun(base_url="https://mgl7.shotgunstudio.com")
>>> sg = sg_obj.sg
>>> print(sg.find.__doc__)

        Find entities matching the given filters.

            >>> # Find Character Assets in Sequence 100_FOO
            >>> # -------------
            >>> fields = ['id', 'code', 'sg_asset_type']
            >>> sequence_id = 2 # Sequence "100_FOO"
            >>> project_id = 4 # Demo Project
            >>> filters = [
            ...     ['project', 'is', {'type': 'Project', 'id': project_id}],
            ...     ['sg_asset_type', 'is', 'Character'],
            ...     ['sequences', 'is', {'type': 'Sequence', 'id': sequence_id}]
            ... ]
            >>> assets= sg.find("Asset",filters,fields)
            [{'code': 'Gopher', 'id': 32, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Cow', 'id': 33, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Bird_1', 'id': 35, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Bird_2', 'id': 36, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Bird_3', 'id': 37, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Raccoon', 'id': 45, 'sg_asset_type': 'Character', 'type': 'Asset'},
             {'code': 'Wet Gopher', 'id': 149, 'sg_asset_type': 'Character', 'type': 'Asset'}]

        You can drill through single entity links to filter on fields or display linked fields.
        This is often called "deep linking" or using "dot syntax".
[...]
```


#### SG 
dummy text
