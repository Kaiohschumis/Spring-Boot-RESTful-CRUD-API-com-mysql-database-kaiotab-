Spring Boot RESTful CRUD API com mysql database (kaiotab)

- Spring Data JPA and Hibernate.
- Spring Web MVC
- RESTful webservices 


Criar tabela no MySQL
CREATE TABLE `product` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `name` varchar(45) NOT NULL,
  `price` float NOT NULL,
  PRIMARY KEY (`id`)
);


curl http://localhost:8080/products
curl http://localhost:8080/products/1


"Content-Type: application/json" -d "{\"id\":1,\"name\":\"iPad\",\"price\":888}" http://localhost:8080/products/1

http://localhost:8080/products/1