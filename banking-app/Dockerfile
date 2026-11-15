# Sử dụng base image JRE 17 Alpine gọn nhẹ
FROM eclipse-temurin:17-jre-alpine

WORKDIR /app

# Sao chép file JAR đã biên dịch vào container
COPY build/libs/*.jar app.jar

# Mở cổng 8080
EXPOSE 8080

# Chạy ứng dụng bằng Exec Form
ENTRYPOINT ["java", "-jar", "app.jar"]
