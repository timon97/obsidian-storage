


##std::all_of()

```cpp
#include <iostream>
#include <algorithm>
using namespace std;

int main() {
	std::vector<int> vec{2,4,6,8,10};
	auto result = std::all_of(vec.begin(), vec.end(), [](const auto& elem){
		return (elem % 2 == 0);
	});

	std::cout << "Result: " << (result ? "true" : "false") << std::endl;
	return 0;
}
```
