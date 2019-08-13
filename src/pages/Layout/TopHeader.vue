<template>
  <md-toolbar md-elevation="0" class="md-transparent">
    <div class="md-toolbar-row">
      <div class="md-toolbar-section-start">
        <h3>Projects</h3>
      </div>
      <div class="md-toolbar-section-end">
        <p>Headphones</p>
        <md-divider vertical></md-divider>
        <md-avatar class="md-avatar-icon md-small">JD</md-avatar>
        <md-avatar class="md-avatar-icon md-small">JD</md-avatar>
        <md-list>
          <md-list-item>
            <md-button>
              <i class="material-icons">star</i>
            </md-button>
          </md-list-item>
          <md-list-item>
            <md-button>
              <i class="material-icons">chat</i>
            </md-button>
          </md-list-item>
          <md-list-item>
            <md-button>
              Reports
            </md-button>
          </md-list-item>
          <div class="md-collapse">
            <div class="md-autocomplete">
              <md-autocomplete
                class="search"
                v-model="selectedEmployee"
                :md-options="employees"
              >
                <label>Search...</label>
              </md-autocomplete>
            </div>
          </div>
          <md-list-item href="#">
            <i class="material-icons">settings</i>
            <p class="hidden-lg hidden-md">Setting</p>
          </md-list-item>
          <md-list-item>
            <md-button>
              <i class="material-icons">arrow_left</i>
              <i class="material-icons">calendar_today</i>
            </md-button>
          </md-list-item>
        </md-list>
      </div>
    </div>
  </md-toolbar>
</template>

<script>
export default {
  data() {
    return {
      selectedEmployee: null,
      employees: [
        "Jim Halpert",
        "Dwight Schrute",
        "Michael Scott",
        "Pam Beesly",
        "Angela Martin",
        "Kelly Kapoor",
        "Ryan Howard",
        "Kevin Malone"
      ]
    };
  }
};
</script>