
## Architecture

### Component Driven Container-View Approach

- Each feature has a separate component which combines view and controller layer for that specific feature and these components can be either used as standalone components or they can be nested into each other to provide a better user interface and code maintainability. 
- Overall app has various Context components which act as containers/wrapper and all other components are rendered inside them. 
- The Context Components also acts as a service layer by interacting with the Recorrido API, and other third-party services like ```Geocode Google Maps Platform API``` available in ```Google Cloud Platform (GCP)```. 
- Thus, all the data received becomes available in global state. 
- Each individual component can then use the global data, this way request-response cycles are reduced thus increasing performance. 
- This availability of global data has been achieved with the help of ```useContext``` React hook.


<img width="994" alt="Screenshot 2024-05-19 at 5 10 18 AM" src="https://github.com/sainishanth17/Mobile-App-Development-Final-Project/assets/107995995/024904d5-bf9a-4b35-9233-5ceb26fc8a5a">
<img width="996" alt="Screenshot 2024-05-19 at 5 10 08 AM" src="https://github.com/sainishanth17/Mobile-App-Development-Final-Project/assets/107995995/9f80a3df-bc67-4005-819d-78085650be68">
<img width="996" alt="Screenshot 2024-05-19 at 5 10 00 AM" src="https://github.com/sainishanth17/Mobile-App-Development-Final-Project/assets/107995995/b383d51c-0ab0-40e1-9df3-5feeee43c56c">
