
```c
// c
#include <locale.h>

// set locale for the calling thread
locale_t uselocale(locale_t newloc);

// set or query the program's current locale
char *setlocale(int category, const char *locale);

// creates a locale object
locale_t newlocale(int category_mask, const char *locale, locale_t base);

// free a locale object
void freelocale(locale_t locobj);

// clones a locale object (for modification)
locale_t duplocale(locale_t locobj);

// translate string
wint_t towctrans(wint_t wc, wctrans_t desc);
wctrans_t wctrans(const char *name);
```