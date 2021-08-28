## Svahaproject Lesson 4
# On top of Lesson 3, we added the following functionalities:
# - Update User information function
# - Enable and disable user function
# - Utilize Fontawesome for icons

## File changed:
# -	UserRepository create updateEnabledStatus method
# -	UserRepositoryTests testDisableUser() and testEnableUser()
# -	UserService create updateUserEnabledStatus method
# -	UserController create updateUserEnabledStatus method
# -	Users.html 
# Modify
 <a th:if=”${user.enabled==true}” class= “fas fa-check-circle fa-2x icon-green”
	Th:href=”@{‘/users/’ +${user.id} + ‘/enabled/false’}”
	Title=”Disable this user”></a>
<a th:if=”${user.enabled==false}” class= “fas fa-circle fa-2x icon-dark”
	Th:href=”@{‘/users/’ +${user.id} + ‘/enabled/true’}”
	Title=”Enable this user”></a>

