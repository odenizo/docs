1. Update the settings for {% data variables.product.github %}'s commit signing service.

   ```bash copy
   sudo consul-template -once -template /etc/consul-templates/etc/nomad-jobs/gpgverify/gpgverify.hcl.ctmpl:/etc/nomad-jobs/gpgverify/gpgverify.hcl
    
   sudo nomad job run /etc/nomad-jobs/gpgverify/gpgverify.hcl
   ```
