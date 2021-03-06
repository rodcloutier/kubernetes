package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
    "go_test",
    "cgo_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "addon_update.go",
        "autoscaling_utils.go",
        "batch_v1_jobs.go",
        "cadvisor.go",
        "cluster_logging_es.go",
        "cluster_logging_gcl.go",
        "cluster_logging_utils.go",
        "cluster_size_autoscaling.go",
        "cluster_upgrade.go",
        "daemon_restart.go",
        "daemon_set.go",
        "dashboard.go",
        "density.go",
        "deployment.go",
        "disruption.go",
        "dns.go",
        "e2e.go",
        "empty.go",
        "empty_dir_wrapper.go",
        "etcd_failure.go",
        "events.go",
        "example_cluster_dns.go",
        "example_k8petstore.go",
        "examples.go",
        "federated-ingress.go",
        "federated-namespace.go",
        "federated-secret.go",
        "federated-service.go",
        "federation-apiserver.go",
        "federation-authn.go",
        "federation-event.go",
        "federation-replicaset.go",
        "federation-util.go",
        "federation-util-14.go",
        "garbage_collector.go",
        "generated_clientset.go",
        "gke_local_ssd.go",
        "gke_node_pools.go",
        "google_compute.go",
        "ha_master.go",
        "horizontal_pod_autoscaling.go",
        "ingress.go",
        "ingress_utils.go",
        "initial_resources.go",
        "job.go",
        "kibana_logging.go",
        "kubectl.go",
        "kubelet.go",
        "kubelet_perf.go",
        "limit_range.go",
        "load.go",
        "logging_soak.go",
        "mesos.go",
        "monitoring.go",
        "namespace.go",
        "networking.go",
        "networking_perf.go",
        "node_problem_detector.go",
        "nodeoutofdisk.go",
        "pd.go",
        "persistent_volumes.go",
        "petset.go",
        "pod_gc.go",
        "portforward.go",
        "pre_stop.go",
        "proxy.go",
        "rc.go",
        "reboot.go",
        "replica_set.go",
        "rescheduler.go",
        "resize_nodes.go",
        "resource_quota.go",
        "restart.go",
        "scheduledjob.go",
        "scheduler_predicates.go",
        "security_context.go",
        "service.go",
        "service_accounts.go",
        "service_latency.go",
        "serviceloadbalancers.go",
        "ssh.go",
        "third-party.go",
        "ubernetes_lite.go",
        "util_iperf.go",
        "volume_provisioning.go",
        "volumes.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//federation/apis/federation/v1beta1:go_default_library",
        "//federation/client/clientset_generated/federation_release_1_5:go_default_library",
        "//federation/pkg/federation-controller/util:go_default_library",
        "//pkg/api:go_default_library",
        "//pkg/api/annotations:go_default_library",
        "//pkg/api/errors:go_default_library",
        "//pkg/api/pod:go_default_library",
        "//pkg/api/resource:go_default_library",
        "//pkg/api/service:go_default_library",
        "//pkg/api/unversioned:go_default_library",
        "//pkg/api/v1:go_default_library",
        "//pkg/apimachinery/registered:go_default_library",
        "//pkg/apis/apps:go_default_library",
        "//pkg/apis/autoscaling:go_default_library",
        "//pkg/apis/batch:go_default_library",
        "//pkg/apis/extensions:go_default_library",
        "//pkg/apis/extensions/v1beta1:go_default_library",
        "//pkg/apis/storage:go_default_library",
        "//pkg/apis/storage/util:go_default_library",
        "//pkg/client/cache:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/core/unversioned:go_default_library",
        "//pkg/client/clientset_generated/release_1_5:go_default_library",
        "//pkg/client/restclient:go_default_library",
        "//pkg/client/transport:go_default_library",
        "//pkg/client/unversioned:go_default_library",
        "//pkg/client/unversioned/clientcmd:go_default_library",
        "//pkg/client/unversioned/clientcmd/api:go_default_library",
        "//pkg/cloudprovider/providers/aws:go_default_library",
        "//pkg/cloudprovider/providers/gce:go_default_library",
        "//pkg/controller:go_default_library",
        "//pkg/controller/deployment/util:go_default_library",
        "//pkg/controller/endpoint:go_default_library",
        "//pkg/controller/job:go_default_library",
        "//pkg/controller/petset:go_default_library",
        "//pkg/fields:go_default_library",
        "//pkg/kubectl:go_default_library",
        "//pkg/kubectl/cmd/util:go_default_library",
        "//pkg/kubelet/api/v1alpha1/stats:go_default_library",
        "//pkg/kubelet/pod:go_default_library",
        "//pkg/labels:go_default_library",
        "//pkg/master/ports:go_default_library",
        "//pkg/metrics:go_default_library",
        "//pkg/registry/generic/registry:go_default_library",
        "//pkg/runtime:go_default_library",
        "//pkg/types:go_default_library",
        "//pkg/util:go_default_library",
        "//pkg/util/exec:go_default_library",
        "//pkg/util/flowcontrol:go_default_library",
        "//pkg/util/intstr:go_default_library",
        "//pkg/util/json:go_default_library",
        "//pkg/util/logs:go_default_library",
        "//pkg/util/net:go_default_library",
        "//pkg/util/runtime:go_default_library",
        "//pkg/util/sets:go_default_library",
        "//pkg/util/system:go_default_library",
        "//pkg/util/uuid:go_default_library",
        "//pkg/util/wait:go_default_library",
        "//pkg/util/workqueue:go_default_library",
        "//pkg/util/yaml:go_default_library",
        "//pkg/version:go_default_library",
        "//pkg/volume/util/volumehelper:go_default_library",
        "//pkg/watch:go_default_library",
        "//plugin/pkg/admission/serviceaccount:go_default_library",
        "//test/e2e/chaosmonkey:go_default_library",
        "//test/e2e/common:go_default_library",
        "//test/e2e/framework:go_default_library",
        "//test/utils:go_default_library",
        "//vendor:github.com/aws/aws-sdk-go/aws",
        "//vendor:github.com/aws/aws-sdk-go/aws/awserr",
        "//vendor:github.com/aws/aws-sdk-go/aws/session",
        "//vendor:github.com/aws/aws-sdk-go/service/autoscaling",
        "//vendor:github.com/aws/aws-sdk-go/service/ec2",
        "//vendor:github.com/elazarl/goproxy",
        "//vendor:github.com/ghodss/yaml",
        "//vendor:github.com/golang/glog",
        "//vendor:github.com/google/cadvisor/info/v1",
        "//vendor:github.com/influxdata/influxdb/client",
        "//vendor:github.com/onsi/ginkgo",
        "//vendor:github.com/onsi/ginkgo/config",
        "//vendor:github.com/onsi/ginkgo/reporters",
        "//vendor:github.com/onsi/gomega",
        "//vendor:github.com/stretchr/testify/assert",
        "//vendor:golang.org/x/crypto/ssh",
        "//vendor:google.golang.org/api/compute/v1",
        "//vendor:google.golang.org/api/googleapi",
        "//vendor:gopkg.in/inf.v0",
        "//vendor:k8s.io/client-go/kubernetes",
        "//vendor:k8s.io/client-go/pkg/api/unversioned",
        "//vendor:k8s.io/client-go/pkg/api/v1",
        "//vendor:k8s.io/client-go/pkg/apis/extensions/v1beta1",
        "//vendor:k8s.io/client-go/pkg/apis/policy/v1alpha1",
        "//vendor:k8s.io/client-go/pkg/util/intstr",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "e2e_test.go",
        "metrics_grabber_test.go",
    ],
    library = "go_default_library",
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/client/unversioned:go_default_library",
        "//pkg/metrics:go_default_library",
        "//test/e2e/framework:go_default_library",
        "//vendor:github.com/onsi/ginkgo",
        "//vendor:github.com/onsi/gomega",
    ],
)
