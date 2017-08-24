node {
  stage "Start"
  checkout scm
  parallel(
    "docker 1": {
      docker.image('node').inside {
        sleep 120
      }
    },
    "docker 2": {
      docker.image('node').inside {
        sleep 180
      }
    }
  )
}
