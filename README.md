基于pytest自动化测试框架

API：接口层/驱动层，根据接口文档编写对应的维护单接口API，提供给测试用例层调用

common：公共方法层，用于放置一些公共方法，如统一加密方法、时间格式转换等

utils：配置层，用于放置一些数据库，host等配置

data：数据层，用于放置测试数据，或根据逻辑算法对数据进行前期准备，数据断言，提供给测试用例层作为接口层的入参进行接口调用

db：数据库层，用于编写sql等提供给测试用例层调用或者断言

test_suitus：测试用例集层，内部会有不同业务线的测试用例层，编写测试用例逻辑，调用API层，进行接口流程自动化测试，并真的测试预期结果进行断言


备注：推荐使用pytest单元测试框架+jenkins持续集成+allure报告，教程见：https://lvjunjie.cn/qa-study/pytest/pytest%E6%8C%81%E7%BB%AD%E9%9B%86%E6%88%90.html
