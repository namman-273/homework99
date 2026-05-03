[ERROR] The goal you specified requires a project to execute but there is no POM in this directory (/home/runner/work/shipping-app/shipping-app). Please verify you invoked Maven from the correct directory.
=>Do trong file yaml,k co actions/checkout.Runner của gh actions khởi tạo máy ảo trống,k checkout cde sẽ k đc tải về =>k tìm thấy file pom


Error:  dependency: ch.qos.logback:logback-classic:jar:9.9.9 (compile)
Error:  	Could not find artifact ch.qos.logback:logback-classic:jar:9.9.9 in central (https://repo.maven.apache.org/maven2)
=>K có phiên bản logback nào như trên

[INFO] --- maven-surefire-plugin:2.12.4:test (default-test) @ shipping-app ---
[INFO] No tests were executed.
=>maven-surefire-plugin phiên bản 2.12.4 đã quá cũ (từ năm 2012), nó không tự động nhận diện và chạy các test của JUnit 5 (junit-jupiter). Để chạy được JUnit 5, cần Surefire version 2.22.0 trở lên.