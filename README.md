# Installation Guide:

**1.Download the **.tar** file [Postman](https://www.postman.com/downloads/)</br>**
**2.Extract the downloaded file by running the following command in **/opt** directory)</br>**
&nbsp;&nbsp;&nbsp; sudo tar -xvzf postman-linux-x64.tar.gz -C /opt</br>
**3.Create a symbolic link running following command in terminal</br>**
&nbsp;&nbsp;&nbsp; sudo ln -s /opt/Postman/Postman /usr/bin/postman</br>
</br>
</br>
**After completing the above process you have successfully installed Postman on your Linux system.</br>
Now to create a desktop icon you can run below command:</br>**

cat << EOF > ~/.local/share/applications/postman2.desktop</br>
[Desktop Entry]</br>
Name=Postman</br>
GenericName=API Client</br>
X-GNOME-FullName=Postman API Client</br>
Comment=Make and view REST API calls and responses</br>
Keywords=api;</br>
Exec=/opt/Postman/Postman</br>
Terminal=false</br>
Type=Application</br>
Icon=/opt/Postman/app/resources/app/assets/icon.png</br>
Categories=Development;Utilities;</br>
EOF</br>
