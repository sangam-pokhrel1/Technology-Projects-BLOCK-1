
## 🧱 Checkpoint 4 — C++ Program (commit: `cpp-basic`)
**Files**: `cpp/main.cpp`

```cpp
#include <iostream>
using namespace std;
int main() {
    int x = 5;
    int y = x + 3;
    cout << "Result: " << y << endl;
    return 0;
}
```
Compile, run, and inspect:
```bash
g++ main.cpp -o main
./main
objdump -d main | head -n 60 > main_cpp.disasm.head.txt
```
**Prompts (add to `journal/04_cpp.md`)**:
- Screenshot with the program output.<img width="4000" height="1800" alt="IMG_20261016_150200" src="https://github.com/user-attachments/assets/1aa4802d-239b-4d2c-88e6-47cb2f6860ad" />

- Compared to C, how does the binary size and disassembly differ (at a glance)? Why might this be?





= The C++ binary may be larger than the C binary because cout and iostream require extra code. The disassembly may also contain more instructions due to C++ library support.
