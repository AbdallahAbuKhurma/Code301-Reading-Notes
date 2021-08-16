# Login and Auth
>
## Review, Research, and Discussion

1. Why is the Context API useful?

        Context provides a way to pass data through the component tree without having to pass props down manually at every level.

2. Can a component outside of a provider get its context?

        It can get global context, cannot get Context.Provider.

3. What are some common use cases for using the Context API?

        Useful for sharing data that can be considered global, such as currently authenticated user, or theme settings for the application

4. Describe “Context Hell”

        Context API has virtually no boilerplate in comparison to Redux, adding Context Providers makes for messy and unreadable code.

## Document the following Vocabulary Terms

* global state :

  * a global state is a set of local states which are all concurrent with each other. A global state in the time domain is also a global state in the causal domain; if two states occur simultaneously, then they cannot have any cause-effect relationship

* global context:

  * This global context is about how concerned we are worldwide, how we make decisions about global issues and how we can act in a responsible way to make the world a better place. The opportunities and tensions provided by world- interconnectedness; The impact

* provider :

  * Provider. Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers.

* consumer:

  * The Consumer component allows a React component to subscribe to the context changes. The component makes the data available using a render prop.

## Preparation Materials

### What is role based access control?

Role-based access control (RBAC) restricts network access based on a person’s role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.

As a result, lower-level employees usually do not have access to sensitive data if they do not need it to fulfill their responsibilities. This is especially helpful if you have many employees and use third-parties and contractors that make it difficult to closely monitor network access. Using RBAC will help in securing your company’s sensitive data and important applications.

### BENEFITS OF RBAC

Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization. Other advantages include:

* Reducing administrative work and IT support. With RBAC, you can reduce the need for paperwork and password changes when an employee is hired or changes their role. Instead, you can use RBAC to add and switch roles quickly and implement them globally across operating systems, platforms and applications. It also reduces the potential for error when assigning user permissions. This reduction in time spent on administrative tasks is just one of several economic benefits of RBAC. RBAC also helps to more easily integrate third-party users into your network by giving them pre-defined roles.

* Maximizing operational efficiency. RBAC offers a streamlined approach that is logical in definition. Instead of trying to administer lower-level access control, all the roles can be aligned with the organizational structure of the business and users can do their jobs more efficiently and autonomously.

* Improving compliance. All organizations are subject to federal, state and local regulations. With an RBAC system in place, companies can more easily meet statutory and regulatory requirements for privacy and confidentiality as IT departments and executives have the ability to manage how data is being accessed and used. This is especially significant for health care and financial institutions, which manage lots of sensitive data such as PHI and PCI data.

### React Cookies

* Cookies are the data stored in the form of key-value pairs that are used to store information about the user on their computer by the websites that the users browse and use it to verify them.

* To set or remove the cookies, we are using a third-party dependency of react-cookie

* Install : npm i react-cookies

* To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie.

## Resources

[what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

[react-cookie library](https://www.npmjs.com/package/react-cookie)
