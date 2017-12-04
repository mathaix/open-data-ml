# open-data-ml

Goal of this project is to create a service that captures statistics on the number of cars that show up in
these RIDot cammeras  http://www.dot.ri.gov/travel/cameras_eastbay.php and store the result in a timeseries database

There are two parts to this project. 

1. Developing a machine model to count cars
Certain amount of research is required. But following projects and papers will provide some initial direction.  
 a. https://pjreddie.com/darknet/yolo/
 b. Paper on counting cars/people in crowded scenes http://agamenon.tsc.uah.es/Investigacion/gram/publications/eccv2016-onoro.pdf
 c. https://research.googleblog.com/2017/06/supercharge-your-computer-vision-models.html
 d. https://tryolabs.com/blog/2017/08/30/object-detection-an-overview-in-the-age-of-deep-learning/
 e. Model could get trained with the TRANCOS dataset http://agamenon.tsc.uah.es/Personales/rlopez/data/trancos/

2. Deploy the service and capturing statistics in a database
Service should continously poll the RI-dot cammera footage and make a call against the developed model to count the cars. 
The captured data should then be stored along with date and time information. 


LICENSE

Copyright 2017 Kenzan, LLC http://kenzan.com

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0
Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
