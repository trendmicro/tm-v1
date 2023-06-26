## Introduction

Trend Vision One™ [Python library (pytmv1)](https://pypi.org/project/pytmv1/)

## Configuration

| Parameter   | Description |
| ----------- | ----------- |
| name        | Identify the application using this library. |
| token       | Authentication token created for your account. |
| url         | Vision One API url this client connects to. |
| pool_connections | Number of connection pools to cache (defaults to 1). |
| pool_maxsize | Maximum size of the pool (defaults to 1). |


## Documentation
### Quick start
### Installation

`pip install pytmv1`

### Usage

----
import pytmv1
client = pytmv1.client("MyApplication", "Token", "https://api.xdr.trendmicro.com")
result = client.get_exception_list()
result.response
GetExceptionListResp(
    next_link=None,
    items=[
        ExceptionObject(
            url='https://*.example.com/path1/*',
            type=<ObjectType.URL: 'url'>,
            last_modified_date_time='2023-01-12T14:05:37Z',
            description='object description'
        )
    ]
)
result.result_code
ResultCode.SUCCESS
----

### Build the project
### Install dependencies

`pip install -e ".[dev]"`

### Build

`hatch build`

### Run unit tests

`pytest --verbose ./tests/unit`

### Run integration tests

`$url`: Vision One API url (i.e: https://api.xdr.trendmicro.com)

`pytest --mock-url="$url" --verbose ./tests/integration`

#### Supported APIs

| Python	| Vision One |
| Connectivity	| |
| `test_connectivity` |	Check availability of service |
| Common	| |
| `get_base_task_result` |	Download response task results |
| `get_task_result` |	Download response task results |
| Domain Account	| |
| `disable_account` |	Disable user account |
| `enable_account` |	Enable user account |
| `reset_password_account` |	Force password reset |
| `sign_out_account` |	Force sign out |
| Email	| |
| `delete_email_message` |	Delete email message |
| `quarantine_email_message` |	Quarantine email message |
| `restore_email_message` |	Restore email message |
| Endpoint	| |
| `collect_file` |	Collect file |
| `isolate_endpoint` |	Isolate endpoint |
| `restore_endpoint` |	Restore endpoint |
| `terminate_process` |	Terminate process |
| Sandbox Analysis	| |
| `download_sandbox_analysis_result` |	Download analysis results |
| `download_sandbox_investigation_package` |	Download investigation package |
| `get_sandbox_analysis_result` |	Get analysis results |
| `get_sandbox_submission_status` |	Get submission status |
| `get_sandbox_suspicious_list` |	Download suspicious object list |
| `submit_file_to_sandbox` |	Submit file to sandbox |
| `submit_urls_to_sandbox` |	Submit URLs to sandbox |
| Search | |
| `get_endpoint_data` `consume_endpoint_data` |	Get endpoint data |
| Suspicious Objects	| |
| `add_to_block_list` |	Add to block list |
| `remove_from_block_list` |	Remove from block list |
| Suspicious Object Exception List	| |
| `add_to_exception_list` |	Add to exception list |
| `get_exception_list` `consume_exception_list` |	Get exception list |
| `remove_from_exception_list` |	Remove from exception list |
| Suspicious Object List	| |
| `add_to_suspicious_list` |	Add to suspicious object list |
| `get_suspicious_list` `consume_suspicious_list` |	List suspicious objects |
| `remove_from_suspicious_list` |	Remove from suspicious object list |
| Workbench	| |
| `add_alert_note` |	Add alert note |
| `edit_alert_status` |	Modify alert status |
| `get_alert_details` |	Get alert details |
| `get_alert_list` `consume_alert_list`	| Get alerts list |

## Contributing
Thank you for your interest in this project, please make sure to read the contribution guide.

## Code of conduct
See Code of conduct.

## License
Project distributed under the [Apache 2.0](https://spdx.org/licenses/Apache-2.0.html) license.