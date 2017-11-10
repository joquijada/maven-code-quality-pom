[Sessions](../jacoco-sessions.md)[maven-code-quality-pom](../index.md)
\> [net.swindle.springdemo.serviceimpl](index.source.md) \>
CloudServiceImpl.java

# CloudServiceImpl.java

``` source lang-java  
package net.swindle.springdemo.serviceimpl;

import java.util.Random;

import net.swindle.springdemo.service.BusinessService;

public class CloudServiceImpl implements BusinessService {

  /* (non-Javadoc)
   * @see net.swindle.springdemo.service.BusinessService#offerService(java.lang.String)
   */
  @Override
  public String offerService(String companyName) {
    final Random random = new Random();
    return "\nAs an Organization, "
        + companyName
        + " offers world class Cloud computing infrastructure."
        + "\nThe annual income exceeds "
        + random.nextInt(revenue)
        + " dollars.";
  }
}
```

Created with [JaCoCo](http://www.jacoco.org/jacoco) 0.7.9.201702052155