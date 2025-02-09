# This Dockerfile will create a image for our spring based java applications 
# Base image 

FROM openjdk:18.0.2.1-jdk
RUN mkdir -p /opt/ali/
ARG JAR_SOURCE
WORKDIR /opt/ali/
COPY ["${JAR_SOURCE}", "/opt/ali/cart-product.jar"]
RUN chmod 777 /opt/ali/
EXPOSE 8132
CMD ["java", "-jar", "/opt/ali/cart-product.jar"]

# /opt/i27/i27cart-product.jar > will be in the container 
