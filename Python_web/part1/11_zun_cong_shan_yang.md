# 1.1 遵从测试山羊的教诲，没有测试什么也别做

在 Python 测试社区中，测试山羊是TDD的非官方吉祥物。

在 TDD 的过程中，第一步始终一样：编写测试

首先要编写测试，然后运行，看是否和预期一样失败，只有失败了才能继续下一步——编写应用程序。

在保存项目代码的地方新建一个 Python 文件，命名为 functional_tests.py，并输入以下代码。

    from selenium import webdriver
    
    browser = webdriver.Firefox()
    
    browser.get('http://localhost:8000')
    
    assert 'Django' in browser.title

