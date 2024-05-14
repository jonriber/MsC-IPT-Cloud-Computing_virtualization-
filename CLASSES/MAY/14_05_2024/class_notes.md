# MAY, 14, 2024 - CLOUD COMPUTING CONSIDERATIONS

## SECURITY CONSIDERATIONS

DISSOLVING PERIMETERS - PREVENTING UNAUTHORIZED ACCESS IN THE CLOUD REQUIRES 
SHIFTING TO A DATA-CENTRIC APPROACH.

Everything is now in software.

Cloud security is a shared responsibility, you are responsible for securing your own space within
cloud.

- use trusted software.
- compliance requirements.
- manage lifecycle
- considering portability
- monitorization
- choosing right people.

Are public clouds secure? --- mitigate risk with hybrid cloud.

Choosing the right security level according to your business rules and your risk management with 
this kind of data.

analogy of renting a building, your relationship with your landlord and neighbours represents how
you handle your cloud application data and access.

## AUDITING N THE CLOUD

On-premises, auditors would sit down with clients and map personnel and physical infra 
to different controls and processes that ought be audited.

On cloud envs, auditing is not that easy. multitenant environment, multiple customers (shared resources),
lack of access to infra because of legal obligations. This is the major reason why companies decide for using 
private clouds.

Compliance is a high priority for cloud providers.


## CLOUD MONITORING AND LOGS

Cloud instances are ephemeral and numerous (scaling out).

centralized logging strategy is mandatory. Use isolated storage area and use standard log formats.

### ELK STACK

- Collect and transform
- Search and Analyze
- Visualize and Manage


## WORST PRACTICES

typical misconceptions when moving to the cloud includes:

- migrating applications to the cloud would be simple that down cost
- companies with inflated expectations due to impressive stories
- misinformation about cloud security. One would think that security is taken care by the provider.
- selecting favorite vendor, not the appropriate one
- not failure ready, considering outages and out-of-business scenarios
- underestimating organizational changes
- skills shortage
- misunderstanding customer requirements

## AUTO SCALING

Ensure you have the correct number of resources to handle current requests.

How to do that?

- group of similar instancs
- set up a desired capacity
- monitoring some parameters on instances
- set of thresholds
- Load balancer
- Vms provisioned
- Monitoring instances mechanism
- API to start and stop VMs
- Reacting scripts according to monitoring services

Most cloud providers offer auto scaling services. Kubernets also provides a Horizontal Pod Autoscaler

Scaling options are used for scaling separeted groups (AWS has it)