<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="card">
        <div class="card-header">
          <h3 class="card-title">Users table</h3>
          <div class="card-tools">
            <button class="btn btn-success">Add User <i class="fas fa-user-plus"></i></button>
          </div>
        </div>
        <!-- /.card-header -->
        <div class="card-body">
          <div id="example2_wrapper" class="dataTables_wrapper dt-bootstrap4">
            <div class="row">
              <div class="col-sm-12 col-md-6"></div>
              <div class="col-sm-12 col-md-6"></div>
            </div>
            <div class="row">
              <div class="col-sm-12">
                <table
                  id="example2"
                  class="table table-bordered table-hover dataTable"
                  role="grid"
                  aria-describedby="example2_info"
                >
                  <thead>
                    <tr role="row">
                      <th
                        class="sorting_asc"
                        tabindex="0"
                        aria-controls="example2"
                        rowspan="1"
                        colspan="1"
                      >Rendering engine</th>
                      <th
                        class="sorting"
                        tabindex="0"
                        aria-controls="example2"
                        rowspan="1"
                        colspan="1"
                      >Browser</th>
                      <th
                        class="sorting"
                        tabindex="0"
                        aria-controls="example2"
                        rowspan="1"
                        colspan="1"
                      >Platform(s)</th>
                      <th
                        class="sorting"
                        tabindex="0"
                        aria-controls="example2"
                        rowspan="1"
                        colspan="1"
                      >Engine version</th>
                      <th
                        class="sorting"
                        tabindex="0"
                        aria-controls="example2"
                        rowspan="1"
                        colspan="1"
                      >Modify</th>
                    </tr>
                  </thead>
                  <tbody>
                    <tr role="row" class="odd">
                      <td class="sorting_1">Gecko</td>
                      <td class>Camino 1.0</td>
                      <td>OSX.2+</td>
                      <td>1.8</td>
                      <td>
                        <a href="#">
                          <i class="fa fa-edit blue"></i>
                        </a>
                        /
                        <a href="#">
                          <i class="fa fa-trash red"></i>
                        </a>
                        
                      </td>
                    </tr>
                  </tbody>
                  <tfoot>
                    <tr>
                      <th rowspan="1" colspan="1">Rendering engine</th>
                      <th rowspan="1" colspan="1">Browser</th>
                      <th rowspan="1" colspan="1">Platform(s)</th>
                      <th rowspan="1" colspan="1">Engine version</th>
                      <th rowspan="1" colspan="1">CSS grade</th>
                    </tr>
                  </tfoot>
                </table>
              </div>
            </div>
          </div>
        </div>
        <!-- /.card-body -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    console.log("Component mounted.");
  }
};
$(document).ready(function() {
  $("#example2").dataTable({
    paging: true,
    lengthChange: true,
    searching: true,
    ordering: true,
    info: true,
    autoWidth: false
  });
});
</script>
