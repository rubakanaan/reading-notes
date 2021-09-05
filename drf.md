# Permissions & Postgresql

### Permissions

* **permissions** : determine whether a request should be granted or denied access
* **Permission** : checks are always run at the very start of the view, before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.
* **Permissions** : are used to grant or deny access for different classes of users to different parts of the API.
* The simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user. This corresponds to the IsAuthenticated class in REST framework.
* A slightly less strict style of permission would be to allow full access to authenticated users, but allow read-only access to unauthenticated users. This corresponds to the IsAuthenticatedOrReadOnly class in REST framework.

## API Reference

#### AllowAny

* The AllowAny permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

* This permission is not strictly required, since you can achieve the same result by using an empty list or tuple for the permissions setting, but you may find it useful to specify this class because it makes the intention explicit.

#### IsAuthenticated
* The IsAuthenticated permission class will deny permission to any unauthenticated user, and allow permission otherwise.

* This permission is suitable if you want your API to only be accessible to registered users.

#### IsAdminUser
* The IsAdminUser permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

* This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.

#### IsAuthenticatedOrReadOnly
* The IsAuthenticatedOrReadOnly will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

* This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.

#### DjangoModelPermissions

* This permission class ties into Django's standard django.contrib.auth model permissions. This permission must only be applied to views that have a .queryset property set. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned.

    * POST requests require the user to have the add permission on the model.
    * PUT and PATCH requests require the user to have the change permission on the model.
    * DELETE requests require the user to have the delete permission on the model.
* The default behaviour can also be overridden to support custom model permissions. For example, you might want to include a view model permission for GET requests.

* To use custom model permissions, override DjangoModelPermissions and set the .perms_map property. Refer to the source code for details.

