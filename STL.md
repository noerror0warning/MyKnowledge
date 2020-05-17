# STL

- find(iterator,iterator,value)，返回value的迭代器
- find_first_of(iterator1,iterator1,iterator2,iterator2)，返回第一个既在1又在2的迭代器
- find_if(iterator,iterator,pre)，返回第一个满足pre的迭代器，pre是函数
- adjacent_find(iterator,iterator,com),返回第一个与邻近关系满足com的迭代器，com是函数
- vector容器中，用emplace_back()插入元素效率会比push_back()高，因为c++11中引入了右值引用，使用前者插入右值时可以少调用一次构造函数
- size()函数返回的是无符号的size_type，使用时注意他可能会向下溢出，例如

  ```
  vector<int> a;
  vector<int> b(2);
  bool c=a.size()-1>b.size()  //这个表达式结果为true
  ```



