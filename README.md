# Android-MVP-Example

 ## What is MVP
 > MVP means that **Model-View-Presenter**.MVP is a derivation of the **Model–View–Controller (MVC)** architectural pattern which mostly used for building user interfaces .In MVP, the presenter assumes the functionality of the **middle-man**. In MVP, all presentation logic is pushed to the presenter.
 ![Image of Android MVP](https://cdn.journaldev.com/wp-content/uploads/2017/08/android-mvp-flow.png)
 
 ## Layer of MVP architecture – Model,View and Presenter
 ### Model
* View have own ViewModel to present data in the view      
* Database Model may be need to retrieve database entity
* Simliery Network model may be to needed represent data entries to retrieve from remote server
* When data move between layer – the Model is transformed from  one layer representation layer to another. 
 ### View
 -> Activity and Fragment and View is passive and can not access model directly.The Views is expose methods which control presentattion of  data or model for instance show or hide certain element.
 ### Presenter
 -> A Presenter is a  middle man between views and Model , It is also contain business logic to the presentation of data.The Presenter the retrive the data from model and format the data before passing the view . The Presenter also update the UI via View
