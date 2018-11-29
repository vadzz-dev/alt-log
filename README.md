# alt-log

## Usage:
```cpp
#include "alt-log.h"

using namespace alt;

int main()
{
  Log::Push(new Log::ConsoleStream);

  Log::Info << "Hello" << Log::Blue << " world" << Log::Endl;
  Log::Warning("Hello", "again");

  return 0;
}
```

```bash
$ g++ -o main main.cpp -std=c++17 && ./main
[19:36:23] Hello world
[19:36:23][Warning] Hello again
```