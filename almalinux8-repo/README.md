TR: AlmaLinux update problemi yaşayan sunucular için aşağıdaki kodları sırasıyla çalıştır.

EN: For servers experiencing AlmaLinux update problems, run the following codes sequentially.

wget -q https://raw.githubusercontent.com/Domainhizmetleri/mixed_code_repository/main/almalinux8-repo/enable-baseurl-almalinux.repo -O /etc/yum.repos.d/almalinux.repo

wget -q https://raw.githubusercontent.com/Domainhizmetleri/mixed_code_repository/main/almalinux8-repo/enable-baseurl-almalinux-powertools.repo -O /etc/yum.repos.d/almalinux-powertools.repo

yum update -y

wget -q https://raw.githubusercontent.com/Domainhizmetleri/mixed_code_repository/main/almalinux8-repo/original-almalinux.repo -O /etc/yum.repos.d/almalinux.repo

wget -q https://raw.githubusercontent.com/Domainhizmetleri/mixed_code_repository/main/almalinux8-repo/original-almalinux-powertools.repo -O /etc/yum.repos.d/almalinux-powertools.repo

reboot
