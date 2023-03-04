---
title: HB Starter Theme
menu:
  main:
    name: Home
    weight: 1
    params:
      icon:
        vendor: bs
        name: house
---

<div class="row">
  <div class="col-12 col-lg-6">
    {{< hb/carousel params.featured=true >}}
  </div>
  <div class="col-12 col-lg-6">
    {{< hb/blog/posts params.pinned=true limit=2 cols="row-cols-2" >}}
  </div>
</div>

<div class="row">
  <div class="col-12 col-lg-8">
    {{< hb/blog/posts sorting="Date desc" limit=6 cols="row-cols-1 row-cols-xl-2" >}}
  </div>
  <div class="col-12 col-lg-4">
    {{< hb/blog/taxonomies limit=20 >}}
  </div>
</div>
