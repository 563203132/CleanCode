### 命名
  + 名副其实，不再需要注释解释
  + 避免误导，不用平台专用名称，提防使用不同处较小的名称，不要用容易混淆的名称I, O <=> 1, 0
  + 做有意义区分
    1. a1, a2 => source, destination
    2. (Product, ProductData, ProductInfo), (moneyAmount, money), (accountData, account)
  + 使用可搜索名称
    1. 单个数字和字母不太好识别， 最好起一个名字 int WORK_DAYS_PER_WEEK = 5;
  + 方法名应为动词或动词短语
    1. postPayment, deletePage, save
    2. 重载构造器，使用描述了参数的静态工厂方法名 Complex.FromRealNumber(23.0); 通常好于 new Complex(23.0);
  + 不要用谚语或俚语起名，难以理解
  + 每个概念对应一个词，contorller, manager和driver有什么区别，为什么不全用其中的一种
  + 别用双关语，
    1. 如很多类中有add方法，它通过增加或连接两个现存值来获取新值，而如果有个方法，把单个参数放到集合，则用insert或append
  + 使用解决方案领域名称，比如访问者模式，AccountVisitor富有含义，比如JobQueue.
  + 用所涉问题领域的名称，可以请教领域专家
  + 加有意义的语境，street,city,state,zipcode放一起明显构成地址，则可以加前缀, addrStreet, addrCity, addrState
  
### 函数
  + 短小， 一个函数几行足矣， if,else和while语句，其中代码只有一行，块内函数拥有较具说明性名称
  + 只做一件事，判断是否在同一个抽象层次上，
    1. TO RenderPageWithSetupAndTearDowns, we check to see whether the page is a test page and if so, we include the setups and teardowns, In either case we render the page in HTML. (此为同一个层次)
  + 
