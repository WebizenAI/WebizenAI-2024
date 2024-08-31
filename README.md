# WebizenAI-2024

This repo is on the 2024 Webizen Local-Host Build.

## What is Webizen Local-Host? 

Webizen Local-Host is a new type of Computing Platform. 

It incorporates a variety of elements, that as am emboidment creates something that is very different to what is currently available in the market, as a form of 'emboidment'.  Whilst the underlying work has been carried out over decades, through which time like-minded individuals have both independently and cooperatively worked to develop various elements, the means to both accomadate recent advancements, challenges and then in-turn (finally) produce the integrated product output, is what this repo is intended to support.

## About Webizen

Webizen, has a history amongst a community of remarkable technologists, who are considered fundamentally, to be human rights advocates.  The need to create foundational Humanitarian ICT infrastructure remains, and is expected to be an on-going challenge. Webizen is now being advanced as a for-purpose activity, where specific goals and design requirements are sought to be achieved within this specific emboidment.

As to encourage and support others means to advance similar forms of work, that may not want to be a member of the webizen ecosystem in a more dedicated manner, efforts to support the production of broader community development through local-host.io and related communities has also been created.  Historically, works were undertaken via the effort termed 'web civics' however after a decade this was considered a failure, remaining unable to support the basic needs of even a single person, whilst others exploited and caused harms, whilst failing to deliver the sorts of outcomes sought to be achieved.  This was an expenive undertaking, that was sadly considered, a defeated failure.

Webizen is being curated with a relatively much smaller focus, whilst still seeking to maintain supports via the webizen community for outcomes considered necessary for Humanitarian ICT related Human Rights supports, as is fundamental to the needs of all members of our human family, and through us, our means to better address issues in our sociosphere; and both, our relationship and capacities to do good, for our biosphere.

## Humanitarian ICT Requirements

Webizen Systems, incorporating both Hardware, Software and Networking requirements, is committed to ensuring support for Humanitarian ICT foundations.  There are many complexities that seemingly fail to be surmised as constituents of common-sense or decency, for many, and we are focused on finding those who do naturally understand; whilst then also, seeking to support the availability to learning materials to help others get a better grasp of concepts that may be considered quite foreign to them.

Some of the qualities, or qualia required, pertains to the characteristics of modern issues, threats and vulnerabilities brought about due to advanced Information Communications Technology ("ICT"), whilst others relate to more traditionally well known and historic considerations, that have traces throughout history in cultures throughout the world over millennia, notwithstanding the difficulties in resourcing aspects pertaining to history even in far shorter time-frames.

Fundamentally, these systems are to ensure that they are not able to be used without available lawful repercussive consequence, for acts relating to digital slavery, intentured survitude, usury and/or breaches to human rights considerations.  Systems are to be designed to ensure that any disputes can be addressed with evidence in a court of law, and the pursuit to both improve supports to protect freedom of thought and both our individual, collective and peacefully cooperative ability to better understand and be empowered by the useful arts and scieces relating to the study of consciousness, health, welfare and causality.

## Innovators - Requirements & Resources

There is a process that seeks to employ considerations relating to duality, where a simultanious effort to produce both supports more broadly via https://local-host.co/ and related channels; as well as, works that are dedicated to webizen specific approaches, is now continuing to be undertaken.  There are specified Hardware Platforms that are sought to be the focus for Webizen works in particular, whilst it is hoped that these works will develop to support components that may not be recommended at this time.

Seperately, the recommendations produced through the development of local-host works more broadly may have alternatives not being pursued or prioritised by Webizen, and this is encouraged but also not the focus of the webizen leadership community.

The Webizen Approach is currently focused on the production of Innovator and Developer focused solutions.  It is believed that this will overtime, lead to refining the solution down to an optimised outcome, that should then be functionally supported by systems that have fewer resources.  Presently, the integration is still a RD&D experimental and creative process, where the definitions continue to be unstable in many areas.  The problems and challenges associated with these works are not simply technical but also social.

### Local-Host Workstation Recommendations

The Local Host / Webizen Workstation Recommendations are defined using the most hardware components most widely supported by the open-source community. Presently, the vast majority of components have been developed for deployment 'on the cloud', whilst other projects have then sought to make them available locally, on traditional computers.

If a participant has an environment that suits the use of rack-mounted systems, there are many benefits, but this is not presently the focus. It is also understood that some of the Apple Mac Mx series systems, in particular the higher-spec'd Mac Studio systems, offer a large amount of vRAM and support for developing apple based ecosystems; however, this is also considered to be an area that Webizen seeks to explore further after the next milestones have been achieved; this may not be the case for local-host.co members.

Some of the GPU options available that are based on AMD or INTEL offerings, alongside other NPU solutions are also of interest in the future, however for the time-being concerns about the means to ensure software support has been taken into consideration and for the time-being, this has led to the recommendation to use nVIDIA.  

Part of the specification focus has been on defining solutions that can provide a Research, Development and Demonstration Environment for under $10,000 AUD (~7k USD) by purchasing 2nd hand parts and putting it together yourself.  Newer solutions are much faster, but are also significantly more expensive at the time.  Due to the focus on Humanitarian ICT, it is known that most people whose work seeks to support these forms of use-cases, will generally find it difficult to afford even the minimum requirements to do meaningful work in this area.  It is expected that these barriers will be reduced in future, as technology advances further.  For the 2024 work, here's my recommendation.

**SPECS:** Minimum Target Specifications are as follows and is subject to change,

**CPUs:** 
- Dual XEON. 24 Cores / 48 Threads
- 2nd Generation Intel Scalable Processors or newer.  https://ark.intel.com/content/www/us/en/ark/products/series/192283/2nd-gen-intel-xeon-scalable-processors.html 
- Support for AVX, AVX2, AVX512, VNNI, AES-NI, Virtualisation.

NOTE: This Configuration provides enough PCI Express Lanes to support multiple GPUs, however one of the more significant limitations is PCIe 3.0 support only.

**RAM:** It is suggested that a minimum of 256GB be assumed, whilst 512GB is preferred. Installation configuration to take-advantage of all available Memory Channels is also advised.

**GPUS:**
- nVidia Ampere Architecture
- Minimum of 72GB of vRAM Recommended.

**NOTE:** GPUs are required for LLM Models, systems and related software functions. Initial Testing shows that most of the LLMs consume less than 40GB RAM, whilst many are under 10GB. There are much larger LLMs that require more than 120GB of vRAM, requiring more complex and more expensive Hardware.  It is believed that it is likely to be more feasible to run the vast majority of systems locally, and then make use of online systems for these more complex tasks if and/or when required.  

GPUs will be consuming the majority of the energy when running and will also generate heat.  Consumer GPUs such as 4090s may not fit into the cases provided for some 2nd hand systems, and may also both produce too much heat and take-up space preventing the installation of additional GPUs, thereby reducing the total amount of vRAM available.  If a LLM model does not have enough vRAM it will not load.  LLMs can be run in System Memory, but are much slower than when operating on GPUs.  nVidia Architectures have developed overtime, and older cards, whilst cheaper, may not support more recent instruction-sets; other 2nd hand cards, designed for data-centre implementations, may not have a cooling solution that is suited for implementation in a workstation.  Whilst i have seen exaples online where 3d printed solutions have been produced, this adds complexity.  

In my case, i found a nVidia a2000 12GB that's used in the system described below; and, 2 x a4000 + 2 x a4500 which i was able to get at a good price, in-part, by describing what i was trying to do with them and my dabilitated financial position generally, alongside knowing how to find 2nd hand components and spending alot of time to find them. 

The benefits of the cards i obtained is that they use less power, have ECC, produce less heat and accumulatively provide 72GB of vRAM (+12GB for the other machine), and therefore fit into the workstation (described below)

**Storage:**
- NvME: 1 - 2 TB NvME for Operating System
- 2 x SSD (1TB+) + 2 x SATA3 (large volume) OR alternative configuration.

NOTE: There are considerations about redundancy (in case of drive-failure), means to perform back-ups (onsite/offsite), the volume of information stored, per user; and the size of databases that are able to be run locally (rather than via online sources) and may also be usefully necessary for local AI related applications & Functions.  However, it is also noted that the access speeds for many of the larger objects, is not a significant problem.

#### Case, PSU, Cooling

The Recommendation is to find an old Workstation made available by Recyclers and 2nd Hand Vendors.  In my case, i've got a Dell Precision 7290, whilst other seemingly good options are available from lenovo, Hewlett Packard and other major vendors, alongside supermicro and other custom builds.  

**PSU:** 
- The Configuration noted above is supported by a 1400w power-supply.  A PSU of between 1300w-2000w is recommended.
- Note: most domestic environments have electricity systems designed for around 2400w (240v/10 Amps).  Overloading can be a hazard.

**Power:** other,
- An energy Monitor is helpful to check whether and how much energy is being used by the system.
- A UPS that can at least ensure a graceful shut-down in case of outage, is recommended.
- If your location has 'dirty power', a full sinewave UPS or converter is recommended, both to protect the system and to reduce the amount of heat generated by the PSU.

**Cooling:**
- The GPUs can easily get hot, and the ability to ensure that there is good ventalation, sufficient air-flow, fans and related considerations is considered essential.  
- Overheating will result in errors, can result in shut-downs and in some cases also, hardware failure.

**Peripherals:** Set-up

The configuration of the systems on this workstation are mostly designed to operate over the network, as such it can be set-up as a network device.  I presently have it set-up as a workstsation, with dual screens, sound, mic, camera, etc.  It is likely that setting it up as a workstation as it is being developed, is probably the best approach.  

**Public Box:** Reception

The notion of a 'receptionist' seek to illustrate the idea of a particular role for interactions with 'the public'. In my case, i am using a hp elitedesk 800 g4 i7 SFF PC, with 32GB ram and the a2000 GPU, as noted previously.  The consideration is, that it may be beneficial for security purposees, to separate the systems that may be used by unauthenticated and/or public 'consumers' online; from, the underlying systems, that may in-turn be storing sensitive personal and private information.  By having two machines, this provides a means where an action must be taken before particular resources are potentially made available to an unintended and/or public user via web-services of the AI agent configured to be running on that device.  This device is also thought helpful for then providing authentication support, to enable access to permissioned information on the Webizen local-host. By having a local device that can support this function, it is believed that far more advanced systems can be operated locally, reducing the need for any online resources and related charges.

Note also, that some LLM related functions are able to run jobs on multiple devices, which means the total available vRAM locally, is also increased.  The addition of another device, also helps to support development related testing across multiple devices, although in my set-up i've also got a laptop, phone, etc.  

**Networking:**

- REQUIREMENT: An internet connection that has greater than 20Mbps / 10Mbps is considered necessary
- RECOMMENDED configuration providing more than 100Mbps / 30Mbps is recommended with at least 1 available static IP.  
- An ethernet connection to the router is also advised if possible, however high-speed wifi is ok.  
- For 'Smart-Home' RD&D, household WiFI is required.  Means to configure the Router is considered a requirement, if this is problematic a 2nd router (network) is suggested.
- A Domain Name is required and a VPS is considered to be likely requirement.  More advanced online services may also be used to provide back-ups of personal files & resources.
- The Networking Environment and related tools, are part of the broader software configuration process.  This will be documented as part of this process.

## Documetation Development

This documentation is being developed. As part of this process, is also, work to improve documentation of components as required to help make it easier for people to get the pieces installed and operating.   One such project is the work on [Openlink Software Virtuoso](https://github.com/WebizenAI/OpenlinkDocs) documentation.  Other elements, include works on [local-host.co](https://local-host.co/) related documentation.  Presently, the objective is to get systems working so that the bulk of the work helping people get involved, is made available within the decentralised networking environment produced and made operational as a result of a successful set-up & install.  

A Keybase group has been set-up for the broader local-host project  [link](https://keybase.io/team/local_host) and selected individuals, stakeholders and/or sponsors, may be invited to join webizen. 