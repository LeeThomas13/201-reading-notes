[DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

Authentication or identification by itself is not usually sufficient to gain access to information or code. For that, the entity requesting access must have authorization.

I sense O auth coming soon...

How Permissions are determined

Before running the main body of the view each permission in the list is checked. If any permission check fails an exceptions.PermissionDenied or exceptions.NotAuthenticated exception will be raised, and the main body of the view will not run.

Object Level Permissions
If you're writing your own views and want to enforce object level permissions, or if you override the get_object method on a generic view, then you'll need to explicitly call the .check_object_permissions(request, obj) method on the view at the point at which you've retrieved the object.

Setting the permission policy

REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}

You can authenticate API's aswell, making it only accessable to registered users.

Third Party Packages

Composed Permissions
The Composed Permissions package provides a simple way to define complex and multi-depth (with logic operators) permission objects, using small and reusable components.

Django Rest Framework Roles
The Django Rest Framework Roles package makes it easier to parameterize your API over multiple types of users.

Django REST Framework API Key
The Django REST Framework API Key package provides permissions classes, models and helpers to add API key authorization to your API. It can be used to authorize internal or third-party backends and services (i.e. machines) which do not have a user account. API keys are stored securely using Django's password hashing infrastructure, and they can be viewed, edited and revoked at anytime in the Django admin.


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)