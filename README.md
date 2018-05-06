# 这是一个测试工程

示例代码：

```java
    public void mkmsg(String str) {
		//handler junk, because thread can't update screen!
		Message msg = new Message();
		Bundle b = new Bundle();
		b.putString("msg", str);
		msg.setData(b);
	    handler.sendMessage(msg);
    }

```

```c

#include "erl_nif.h"

#define DEBUG 0

static ERL_NIF_TERM atom_ok;
static ERL_NIF_TERM atom_error;

static int load(ErlNifEnv* env, void** priv_data, ERL_NIF_TERM load_info) {
  atom_ok    = enif_make_atom(env, "ok");
  atom_error = enif_make_atom(env, "error");
  return 0;
}

```
![asldfjas](https://timgsa.baidu.com/timg?image&quality=80&size=b9999_10000&sec=1525576630284&di=0968503aac065f4d334454e3325d3587&imgtype=0&src=http%3A%2F%2Fimg.zcool.cn%2Fcommunity%2F038c0ee5744f9a500000025ae5acd2a.jpg)