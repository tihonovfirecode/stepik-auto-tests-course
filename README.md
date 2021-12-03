# stepik-auto-tests-course
Первые шаги в освоении
https://stepik.org/lesson/187065/step/7?auth=login&unit=161976

    catalog_button = browser.find_element_by_css_selector('div.catalog-button').click()
    razdel = random.randint(1, 6)
    time.sleep(2)
    if razdel == 1 :
        razdel = 'Книги'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(1)').click()
        time.sleep(2)
        browser.execute_script("window.scrollTo(0, 500)")
    elif razdel == 2 :
        razdel = 'Канцтовары'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(2)').click()    
    elif razdel == 3 :
        razdel = 'Сувеиры'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(3)').click()
    elif razdel == 4 :
        razdel = 'Игры и игрушки'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(4)').click()
    elif razdel == 5 :
        razdel = 'Календари'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(5)').click()
    elif razdel == 6 :
        razdel = 'Творчество'
        catalog_knigi = browser.find_element_by_css_selector('div.categories-menu div.main-category:nth-of-type(6)').click()
    print('Переход в раздел :', razdel)  

