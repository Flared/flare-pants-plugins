resources(
    name="package_data", sources=["pyproject.toml", "LICENSE-MIT.txt"]
)

python_distribution(
    name="package",
    dependencies=[
        ":package_data",
        "./flare_protobuf_plugin:flare_protobuf_plugin@resolve=pants-plugins",
    ],
    provides=python_artifact(
        name="flare_protobuf_plugin",
        version="0.1.0",
    ),
    repositories=[
      "@pypi",
    ]
)
