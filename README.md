# Пример Service Locator

## Создаём компанент как Service Locator и прекрепляем его глобально к экземпляру приложения, так чтобы он был доступен 
по Yii::$qpp->serviceLocator


Вместо того чтобы вручную создавать экземпляры различных общих служб (компонентов приложения), мы можем получить 
их из специального глобального объекта, который содержит конфигурации и экземпляры всех компонентов. 
Локатор служб-это глобальный объект, который содержит список компонентов или определений, однозначно 
идентифицируемых по идентификатору, и позволяет получить любой необходимый экземпляр по его идентификатору. 
Локатор создает один экземпляр компонента "на лету" при первом вызове и возвращает предыдущий экземпляр при 
последующих вызовах. В этом рецепте мы создадим компонент корзины и напишем контроллер корзины для работы с ним.

