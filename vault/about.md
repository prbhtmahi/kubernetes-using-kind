Ref repo: github.com/scriptcamp/kubernetes-vault.git

What?

HashiCorp Vault is an identity-based secrets and encryption management system. It provides
  encryption services that are gated by authentication and authorization methods to ensure secure , auditable and restricted access to secrets.


  how it works?

  Vault works primarily with token and a token is associated to the client's policy. Each policy is 
  path-based and policy rules constrains the actions and accessibility to the paths for each client.
  With vault, you can create tokens manually and assign them to client.


  why?

  As kubernetes default secret object is just base64 encoded. we need a good secret management tool and workflow to
   manage secret storage and retrieval for production use cases.



   SetUp...


   Vault RBAC Setup::::

   a. ClusterRoles:- Kubernetes clusterRoles are entites that have been assigned certain special permissions.

   b. ServiceAccounts: kubernetes serviceAccounts are identities assigned to entities such as pods to enable their interation with the kubernetes APIs using the role's permissions.

   c. ClusterRoleBinding: ClusterRoleBinding are entities that provide roles to accounts i.e. they grant permission to service accounts.
