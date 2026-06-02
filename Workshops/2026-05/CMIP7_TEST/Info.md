CMIP7 Test Data on Levante can be found under
/work/bd0854/DATA/ESMValTool2/CMIP7_DUMMY_DATA/

The config file entry would be:
```
CMIP7:
    data:
      dkrz_test:
        type: esmvalcore.io.local.LocalDataSource
        rootpath: /work/bd0854/DATA/ESMValTool2/CMIP7_DUMMY_DATA
        # Directory structure and file name template from https://wcrp-cmip.github.io/cmip7-guidance/CMIP7/global_attributes/
        dirname_template: "{drs_specs}/{project}/{activity}/{institute}/{dataset}/{exp}/{ensemble}/{region}/{frequency}/{short_name}/{branding_suffix}/{grid}/{version}"
        filename_template: "{short_name}_{branding_suffix}_{frequency}_{region}_{grid}_{dataset}_{exp}_{ensemble}*.nc"
```
