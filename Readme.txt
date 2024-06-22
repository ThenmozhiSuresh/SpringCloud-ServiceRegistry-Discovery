Step1:
1.CustomerService act as a Eureka server - @EnableEurekaServer
2.Self Eureka registration is not needed So register-with-eureka : false
3.Port running : 8070
4.Application name : CUSTOMER-SERVICE

//Now we can open & view Erueka dashboard with 0 instances.

Step2:
1.Payment service act as Eureka Client - @EnableEurekaClient
2.simple controller to return Some String
3.Lets register this service in Eureka server
4.registerWithEureka : true
  Eureka server url (defaultZone: http://localhost:8070/eureka/)
5.Application Name : PAYMENT-SERVICE

//Lets open & view Eureka server Now we can see--> Eureka Client-payment-service
Now create multiple instances for payment & we can able to see all those payment Instances & their individual status

Step3:
1.same way create one more Eureka client -  SHOPPING-SERVICE
Register those & view in Eureka server


